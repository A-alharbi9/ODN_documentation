# Web App Specifications

This document describes the specifications for both the website and web client. The website is the public facing website that is used to promote the Open Dev Net project. The web client is the web application that is used to interact with the Open Dev Net platform.

## Technologies

There are several technologies that will be used to build the web app, each of which are recommended for developers to have solid experience with before contributing to **relevant** parts of the project, These include:

- TypeScript – Programming language.
- Next.js – Primary frontend framework.
- Redux – State management.
- TailwindCSS – CSS framework for styling.
- UI library – ODN UI.
- Docker – Create a containerized environment for the web app to run in.
- Git/GitHub – Version control and project code management.

Other technologies include JSON to interact with the backend API, JWT for authentication, and WebSocket for live connections.

## UI Design

UI designs and UX flows are available on Figma. The designs are publically available for viewing and commenting, but only contributors can edit the designs.

An internal UI library (odn-ui) is used for consistent styling and components across the web app. The UI library is built using TailwindCSS and React.

## Pages

Different screeens are considered pages, each with a unique route. The following pages are required for the web app:

### Website

| Page             | Path          | Brief Description                                                          |
| ---------------- | ------------- | -------------------------------------------------------------------------- |
| Home             | `/`           | Shows a preview of the platform and advertises some of it's core features. |
| About            | `/about`      | Information about the project and the team behind it.                      |
| Contact          | `/contact`    | Contact information for the project.                                       |
| Blog             | `/blog`       | Blog posts about the project.                                              |
| Login            | `/login`      | Allows users to login to the platform.                                     |
| Register         | `/register`   | Allows users to register for the platform.                                 |
| Help             | `/help`       | Provides help and support for the platform.                                |
| Privacy Policy   | `/privacy`    | The privacy policy document.                                               |
| Terms of Service | `/terms`      | The terms of service document.                                             |
| Guidelines       | `/guidelines` | The community guidelines document.                                         |
| Documentation    | `/docs`       | Shows the documentation for the platform.                                  |

### Web Client

| Page     | Path              | Brief Description                                                                                          |
| -------- | ----------------- | ---------------------------------------------------------------------------------------------------------- |
| App      | `/`               | The main page of the web client. Shows the user's dashboard and allows them to navigate to other sections. |
| Explore  | `/explore`        | Place for users to find new guilds and projects.                                                           |
| User DM  | `/dm/{user.id}`   | Place for users to chat with other users.                                                                  |
| Group DM | `/dm/{group.id}`  | Place for users to chat with other users.                                                                  |
| User     | `/user/{user.id}` | A user's full profile.                                                                                     |

**User**

| Page                       | Path                        | Brief Description                                  |
| -------------------------- | --------------------------- | -------------------------------------------------- |
| Friends                    | `/friends`                  | Where users can view and manage their friends.     |
| Settings                   | `/settings`                 | Where users can edit their settings.               |
| Settings - Profile         | `/settings/profile`         | Where users can edit their profile.                |
| Settings - Account         | `/settings/account`         | Where users can edit their account.                |
| Settings - Privacy         | `/settings/privacy`         | Where users can edit their privacy settings.       |
| Settings - Security        | `/settings/security`        | Where users can edit their security settings.      |
| Settings - Notifications   | `/settings/notifications`   | Where users can edit their notification settings.  |
| Settings - Appearance      | `/settings/appearance`      | Where users can edit their appearance settings.    |
| Settings - Accessibility   | `/settings/accessibility`   | Where users can edit their accessibility settings. |
| Settings - Connections     | `/settings/connections`     | Where users can edit their connections.            |
| Settings - Billing         | `/settings/billing`         | Where users can edit their billing settings.       |
| Settings - Authorized Apps | `/settings/authorized-apps` | Where users can edit their authorized apps.        |

**Guild**

| Page                          | Path                                      | Brief Description                                               |
| ----------------------------- | ----------------------------------------- | --------------------------------------------------------------- |
| Create New Guild              | `/guild/new`                              | Page for creating a new guild.                                  |
| Guild                         | `/guild/{guild.id}`                       | Home page for a specific guild.                                 |
| Guild Channel                 | `/guild/{guild.id}/channel`               | A channel within a guild.                                       |
| Guild Settings - Overview     | `/guild/{guild.id}/settings`              | Configure basic info, such as the guild's type, name, and icon. |
| Guild Settings - Appearance   | `/guild/{guild.id}/settings/appearance`   | Configure the guild's theme.                                    |
| Guild Settings - Roles        | `/guild/{guild.id}/settings/roles`        | Configure roles and permissions.                                |
| Guild Settings - Assets       | `/guild/{guild.id}/settings/assets`       | Configure emojis and stickers.                                  |
| Guild Settings - Members      | `/guild/{guild.id}/settings/members`      | View and manage guild members.                                  |
| Guild Settings - Bans         | `/guild/{guild.id}/settings/bans`         | Where guild admins can edit guild bans.                         |
| Guild Settings - Applications | `/guild/{guild.id}/settings/applications` | Where guild admins can edit guild applications.                 |
| Guild Settings - Moderation   | `/guild/{guild.id}/settings/moderation`   | Where guild admins can edit guild moderation settings.          |
| Guild Settings - Audit Logs   | `/guild/{guild.id}/settings/audit-logs`   | Where guild admins can view guild audit logs.                   |
| Guild Settings - Invites      | `/guild/{guild.id}/settings/invites`      | Where guild admins can view guild invites.                      |
| Guild Settings - Analytics    | `/guild/{guild.id}/settings/analytics`    | Where guild admins can view guild analytics.                    |
