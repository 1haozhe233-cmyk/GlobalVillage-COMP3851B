# Global Village

Source code for the COMP3851B Global Village team project. The application uses Flutter for the client and separate authentication, community, chat, and family services. Community features include nearby people, activities, activity group chats, and notifications.

Live website: https://global-village-haozhe.malaysiawest.cloudapp.azure.com/

## Source layout

- `lib/`, `web/`, `android/`, `test/`: Flutter app and tests
- `auth-server/`, `chat-server/`, `family-server/`, `server/`, `public-gateway/`: backend services
- `auth-database/`: database setup
- `docker-compose.public.yml`: deployment services
- `DEVELOPMENT_HANDOFF.md`: development and setup notes

## Build

Install Flutter and Docker. Copy the relevant `.env.example` files to local `.env` files and supply your own credentials. Run `flutter pub get` and `flutter build web` from the repository root. The production gateway and services are defined in `docker-compose.public.yml`; see `DEVELOPMENT_HANDOFF.md` for local setup details.

This repository is a source snapshot. Runtime databases, generated builds, local environment files, and private credentials are excluded.
