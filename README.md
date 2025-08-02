# Multiplayer Career Limiting Maneuver

A multiplayer globe app where you can see who else is "pulling a Career Limiting Maneuver™" in real time! Built with Cloudflare Workers, Durable Objects, and PartyKit, this site visualizes visitors as markers on a spinning globe—with a few fun surprises.

## Features

- Real-time globe showing all connected users as markers

## How It Works

- Each visitor opens a WebSocket connection to a Durable Object, which manages the globe state.
- When a user joins or leaves, all clients are updated in real time.
- The globe is rendered with [Cobe](https://cobe.vercel.app/), and the backend is powered by Cloudflare Durable Objects and PartyKit.

## Getting Started

1. Install dependencies:
   ```bash
   pnpm install
   ```
2. Start the local development server:
   ```bash
   pnpm dev
   ```
   This uses Wrangler to build and serve the Worker and static assets.
3. Deploy to Cloudflare:
   ```bash
   pnpm deploy
   ```

## License

MIT. See [LICENSE](./LICENSE) for details. Attribution for Cobe, Phenomenon, and PartyServer is preserved in the codebase.

## Credits

This project is based on the [Cloudflare Multiplayer Globe Template](https://github.com/cloudflare/templates/tree/v5.1.0/multiplayer-globe-template).
