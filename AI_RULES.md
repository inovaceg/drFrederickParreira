# AI Development Rules

## Tech Stack

• **Frontend**: React with TypeScript
• **Styling**: Tailwind CSS with shadcn/ui components
• **Routing**: React Router
• **Backend**: Supabase (auth, database, edge functions)
• **UI Components**: Prefer shadcn/ui library components
• **Icons**: Use lucide-react icon library
• **State Management**: React hooks and context
• **Data Fetching**: Supabase client for database operations
• **Authentication**: Supabase Auth with @supabase/auth-ui-react
• **Realtime**: Supabase Realtime subscriptions

## Library Usage Rules

### UI & Styling
• **Always use** Tailwind CSS for styling instead of plain CSS
• **Prefer shadcn/ui components** for common UI elements (buttons, forms, cards, etc.)
• **Use lucide-react** for all icons instead of other icon libraries
• **Avoid** installing additional UI/component libraries unless absolutely necessary

### Backend & Data
• **Use Supabase client** for all database operations
• **Use Supabase Auth** for all authentication needs
• **Use Supabase Edge Functions** for server-side logic
• **Avoid** direct database connections or custom backend servers

### Routing & Navigation
• **Use React Router** for all client-side routing
• **Follow file structure**: pages in `src/pages`, components in `src/components`

### State Management
• **Use React hooks** (useState, useEffect, useContext) for state management
• **Use Supabase Realtime** for live updates instead of polling
• **Avoid** external state management libraries like Redux unless specifically required

### Forms & Validation
• **Use react-hook-form** for form handling (included with shadcn/ui)
• **Use zod** for validation schemas (included with shadcn/ui)

### Notifications
• **Use react-hot-toast** for toast notifications (already configured)
• **Use shadcn/ui alert dialogs** for confirmation dialogs

### Data Visualization
• **Use recharts** for charts and graphs (already configured with shadcn/ui)
• **Avoid** installing additional charting libraries

### Authentication
• **Use @supabase/auth-ui-react** for login/signup UI
• **Use Supabase Auth utilities** for session management
• **Avoid** third-party authentication libraries

### API Calls
• **Use Supabase client methods** for database queries
• **Use Supabase Edge Functions** for custom server-side logic
• **Avoid** fetch/axios for direct API calls to backend

### File Structure
• **Pages**: `src/pages/` directory
• **Components**: `src/components/` directory
• **Supabase Integration**: `src/integrations/supabase/` directory
• **Utilities**: `src/utils/` directory
• **Hooks**: `src/hooks/` directory
• **Edge Functions**: `supabase/functions/` directory