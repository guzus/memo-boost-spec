# Memo-Boost

> "Not your server, not your data."

**Memo-Boost** is an open-source self-custodial data management framework.

- Mitigates trust factors when storing and using data.
- Users have flexibility to customize memo-boost according to their requirements.

## Memo-Boost Architecture

memo-boost consists of three modules: `Client, Relay, Database`.

Users should host their own and `Relay` (essential), `Database` (essential) and `Client` (optional).

### 1. Client

Client is a user-friendly module for users to easily create, read, update, delete their data at anytime anywhere.

Diversity of Write Client could be implemented, such as

- bookmarking chrome extension (similar to Pocket / Instapaper)

- telegram bot that stores every messages in specific Telegram chatroom

- importing data from other sources

For Read Client, DBMS like DBeaver are good enough, but we can imagine more for instance:

- memo summarization, visualization, brainstorm-assisting tool using AI

- paying crypto to subscribe to other's memos

- exporting data in csv form

### 2. Relay

Relay is a middleware between clients and database to facilitate clients interacting with database.

### 3. Database

Database stores your private data.

## Repositories

Not yet implemented.
- [memo-boost-client]()
- [memo-boost-relay]()
- [memo-boost-database]()

## FAQ

### Why not use existing services like Pocket, Instapaper, Evernote, Notion, etc?

- 1 - They are centralized, so you have to trust them to store your data. (They can track your bookmarks, who knows?) 2 - They aren't fully open-source, so the data compatibility between services are not guaranteed. (e.g. you can't export your memo from Pocket to Google Keep)

### Where do I host Client, Relay, Database?

- You can host them on your home server, or use cloud services like AWS, GCP, Azure, etc. Of course you can host Relay and Database in a single server. Every scenario should be considered when contributing to memo-boost.

## Contribution Guidelines

Check out [CONTRIBUTION.md](./CONTRIBUTION.md)
