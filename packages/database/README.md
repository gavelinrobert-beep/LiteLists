# @litelists/database

This package contains Supabase database schema definitions, migrations, and seed data for LiteLists.

## Structure

```
/database
  /migrations        # Supabase migration files
  /seeds             # Seed data for development
  /types             # Generated TypeScript types from database schema
  README.md          # This file
```

## Setup

Database migrations are managed using the Supabase CLI.

### Prerequisites

- Supabase CLI installed (`brew install supabase/tap/supabase` or via npm)
- Supabase project created at https://supabase.com

### Local Development

```bash
# Initialize Supabase locally (from project root)
supabase init

# Start local Supabase instance
supabase start

# Create a new migration
supabase migration new <migration_name>

# Apply migrations
supabase db push

# Reset database (WARNING: deletes all data)
supabase db reset
```

### Production Deployment

```bash
# Link to your Supabase project
supabase link --project-ref <project-id>

# Push migrations to production
supabase db push

# Generate TypeScript types
supabase gen types typescript --linked > types/database.types.ts
```

## Schema Overview

The database schema will include:

- **users** - User profiles and authentication
- **spaces** - Households/groups (e.g., "Home", "Vacation")
- **space_members** - Join table for users in spaces
- **lists** - Shopping/packing lists within spaces
- **list_items** - Individual items on lists
- **activities** - Activity feed for list changes
- **invites** - Invitation links and QR codes for joining spaces

## Real-time Subscriptions

Tables configured for real-time updates:
- `list_items` - Real-time item updates
- `lists` - List metadata changes
- `activities` - Activity feed updates

## Row-Level Security (RLS)

All tables use Supabase RLS policies to ensure:
- Users can only access spaces they're members of
- List items are only visible to space members
- Proper authorization for all CRUD operations
