---
title: Roadmap
enableTableOfContents: true
tag: updated
redirectFrom:
  - /docs/cloud/roadmap
  - /docs/conceptual-guides/roadmap
  - /docs/reference/roadmap
updatedOn: '2025-05-09T22:43:28.155Z'
---

Our development teams are focused on helping you ship faster with Postgres. This roadmap describes committed features we're working on right now, what we delivered recently, and a peek at what's on the horizon.

## What we're working on now

Here's a snapshot of what we're working on now:

- **Postgres for AI agents**: [Replit partnered with Neon to back Replit Agents](https://neon.tech/blog/looking-at-how-replit-agent-handles-databases), creating thousands of Postgres databases. If you're building AI agents and would like to integrate agent-ready Postgres, [connect with us](https://neon.tech/agent-design-partner). See [Postgres for AI Agents](https://neon.tech/use-cases/ai-agents) for more.
- **Backup & restore**: We'll start with scheduled snapshots with instant point-in-time recovery, eventually expanding this feature with more traditional automated backup capabilities.
- **Data API**: We're working on a Data API feature, powered by PostgREST.
- **Monitoring platform support**: After adding [Datadog integration](/docs/guides/datadog#steps-to-integrate-datadog-with-neon) in 2024, we're planning support for additional monitoring platforms.
- **Larger computes GA**: Autoscaling up to 16 vCPUs and fixed compute sizes up to 56 vCPUs are currently in Beta; GA support is planned for 2025.
- **Console navigation improvements**: Enhancing navigation for multi-project organizations, branch clarity, and better SQL Editor and Tables page interactions.
- **Claimable Databases**: A new way for SaaS vendors to partner with Neon to offer instant Postgres databases. Let your users create Postgres databases — no registration required.

Other features you would like to see? [Let us know](#share-your-thoughts).

## What's on the horizon

And here's a quick list of what we'll be taking on in the near future:

- **Private Networking on Azure**: Following on [AWS PrivateLink support](/docs/guides/neon-private-networking), Azure Private Link is next.
- **More Auth provider support for Neon Auth**: This feature lets you sync user profiles from your auth provider to your database automatically. See [Neon Auth](/docs/guides/neon-identity) for details.

## What we've shipped recently 🚢

- **Neon on Azure GA**: We've announced our general availability release on Azure with deeper Azure integration. [Read the announcement](https://neon.tech/blog/azure-native-integration-ga).
- **Improved migration assistance**: The [Import Data Assistant](/docs/import/import-data-assistant) makes data import easier and faster.
- **Data anonymization**: We've added support for the PostgreSQL Anonymizer extension (`anon`). [Learn more](/docs/guides/neon-auth).
- **Neon serverless driver GA**: Our JavaScript/TypeScript serverless driver has reached version 1.0.0, bringing stronger SQL injection safeguards and better performance for serverless environments.
- **Neon Snapshots (Early Access)**: Create and manage point-in-time copies of your database with our new unified Backup & Restore experience.
- **Inbound logical replication GA**: Neon now fully supports Postgres logical replication for inbound data (replicating data to Neon).
- **Postgres logs in Datadog (Beta)**: Stream and analyze your Postgres logs directly in your Datadog dashboard for better observability. Available on Scale and Business plans.
- **Support for [pg_search](https://neon.tech/docs/extensions/pg_search)**: We partnered with [ParadeDB](https://www.paradedb.com/) to bring `pg_search` to Neon, delivering up to 1,000x faster full-text search inside Postgres on versions 14, 15, and 16. [Read the announcement](https://neon.tech/blog/pgsearch-on-neon).
- **MACC-eligibility on Azure**: Neon Postgres purchases made through the Azure Marketplace are now counted toward your Microsoft Azure Consumption Commitment (MACC). [Learn more](https://neon.tech/docs/introduction/billing-azure-marketplace#microsoft-azure-consumption-commitment-macc).
- **GitHub Secret Scanning**: Neon joined GitHub's Secret Scanning Partner Program to automatically detect and protect against exposed database credentials in public repositories.
- **HIPAA compliance**: We have achieved HIPAA compliance. Learn more about Neon's compliance milestones on our [Compliance page](/docs/security/compliance).
- **Scheduled updates**: Business plan users can now check for update notices and choose preferred update windows for Postgres updates, security patches, and Neon feature enhancements.
- **AWS São Paulo region**: Create projects in São Paulo (sa-east-1) for lower latency access from the South America and data residency within Brazil.
- **Vercel preview deployment support**: We added support for preview deployments to our **Vercel Native Integration**. See [Vercel Native Integration Previews](/docs/guides/vercel-native-integration-previews).
- **Manage your database from Cursor or Claude Desktop**: Manage your Neon database directly from [Cursor](https://neon.tech/guides/cursor-mcp-neon) or [Claude Desktop](https://neon.tech/guides/neon-mcp-server) using natural language, made possible by the [Neon Model Context Protocol (MCP) Server](https://github.com/neondatabase/mcp-server-neon).
- **Database Branching for Vercel Preview Environments**: We added support for **database branching for preview environments** to the **Neon Postgres Native Integration**, available from the [Vercel Marketplace](https://vercel.com/marketplace).
- **AWS London region**: Create projects in London (eu-west-2) for lower latency access from the UK and data residency within the United Kingdom.
- **Datadog integration GA**: Monitor your Neon database performance, resource utilization, and system health directly from Datadog's observability platform.
- **Save your connection details to [1Password](https://1password.com/)**: See [Save your connection details to 1Password](/docs/connect/connect-from-any-app#save-your-connection-details-to-1password).
- **Query monitoring in the console**: Monitor your [active queries](/docs/introduction/monitor-active-queries) and [query history](/docs/introduction/monitor-query-history) in the Neon Console.
- **The Neon App for Slack**: Stay connected to your Neon Serverless Postgres databases in Slack. See [Neon App for Slack](/docs/manage/slack-app).
- **Schema-only branches**: Create branches that include only your database schema—ideal for workflows involving sensitive data. This feature is now available in Early Access. [Learn more](/docs/guides/branching-schema-only).
- Support for the [postgres_fdw](/docs/extensions/postgres_fdw), [dblink](https://neon.tech/docs/extensions/dblink), and [pg_repack](/docs/extensions/pg_repack) Postgres extensions.
- **"Instagres": No signup, instant Postgres**: An app that lets you generate a Postgres database URL almost instantly — no sign up required. Give it a try at [https://www.instagres.com/](https://www.instagres.com/) or by running `npx instagres` in your terminal. See how fast Neon can spin up a Postgres database (AI agents loves this, btw).
- **Neon Chat for Visual Studio Code**: This AI-powered assistant lets you chat with the latest Neon documentation without leaving your IDE. You can find it here: [Neon Postgres VS Code Extension](https://marketplace.visualstudio.com/items?itemName=buildwithlayer.neon-integration-expert-15j6N).
- **A GitHub Copilot extension**: This extension provides chat-based access to the latest Neon documentation directly from your repository. You can find it here: [Neon Postgres Copilot Extension](https://github.com/marketplace/neon-database)
- **Schema Diff API**: Neon now supports schema checks in agentic systems and deployment pipelines with the new schema diff API endpoint. Learn more about [Schema Diff](/docs/guides/schema-diff), which is also available via the console and CLI.
- **Neon Auth (Early Access)**: Sync user profiles from your auth provider to your database automatically. Currently in Early Access. See [Neon Auth](/docs/guides/neon-auth) for details.
- **Postgres 17**: Now the default version for all newly created projects.
- **Support for [pg_cron](/docs/extensions/pg_cron)**: Schedule and manage periodic jobs directly in your Postgres database with this extension.
- **Neon on AgentStack**: Integrate Neon with AgentStack to enable AI agents to create ephemeral or long-lived Postgres instances for structured data storage. Explore the [Neon tool](https://github.com/AgentOps-AI/AgentStack/blob/main/agentstack/_tools/neon/__init__.py) in AgentStack's repo.
- **Neon on Composio**: Integrate Neon's API with LLMs and AI agents via Composio. Check out the [Composio integration](https://composio.dev/tools?search=neon).
- **Higher connection limits for autoscaling configurations**: Postgres `max_connections` are now much higher. [Learn more](/docs/connect/connection-pooling#connection-limits-without-connection-pooling).
- **PgBouncer `default_pool_size` scaling**: The `default_pool_size` is now set according to your compute's `max_connections` setting. Previously, it was fixed at `64`. [Learn more](/docs/connect/connection-pooling#neon-pgbouncer-configuration-settings).
- **Neon Auth.js Adapter**: Simplify authentication with the new [Auth.js Neon Adapter](https://authjs.dev/getting-started/adapters/neon).

<details>
<summary>Shipped in 2024</summary>

- **Larger computes**: Autoscaling now supports up to 16 vCPUs, and fixed compute sizes up to 56 vCPUs are available in Beta.
- **A Model Context Protocol (MCP) server for Neon**: We released an open-source MCP server, enabling AI agents to interact with Neon's API using natural language for tasks like database creation, SQL queries, and migrations. Read the blog post: [Let Claude Manage Your Neon Databases: Our MCP Server is Here](https://neon.tech/blog/let-claude-manage-your-neon-databases-our-mcp-server-is-here).
- **Neon in the Azure Marketplace**: Neon is now available as an [Azure Native Integration](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/neon1722366567200.neon_serverless_postgres_azure_prod?tab=Overview), enabling developers to deploy Neon Postgres databases directly from the Azure portal. [Read the announcement](https://neon.tech/blog/neon-is-now-available-as-an-azure-native-integration).
- **Archive storage on paid plans**: To minimize storage costs on paid plans, we now support automatic archiving of inactive branches (snapshots of your data) in cost-efficient object storage. For more about this feature, see [Branch archiving](/docs/guides/branch-archiving).
- **Organizations GA**: Organization Accounts are now generally available. Create a new organization, transfer over your projects, invite your team and get started collaborating. Refer to our [Organizations docs](/docs/manage/organizations) to learn more.
- **Private Networking**: Private and secure network access to your compute resources without traversing public networks. Support for AWS PrivateLink is available in [Public Beta](/docs/guides/neon-private-networking).
- **Schema Diff GitHub Action**: This action leverages our [Schema Diff](/docs/guides/schema-diff) feature to compare database schemas across branches and post the differences as a comment on your pull request, streamlining the review process. It's also supported with our [Neon GitHub integration](/docs/guides/neon-github-integration).
- **Import Data Assistant**: Helps you migrate data to Neon from other Postgres databases. All you need to get started is a connection string for your existing database. See [Import Data Assistant](/docs/import/import-data-assistant) for instructions.
- **Python SDK**: Our new [Python SDK](https://pypi.org/project/neon-api/) wraps the [Neon API](https://api-docs.neon.tech/reference/getting-started-with-neon-api), allowing you to manage the Neon platform directly from your Python applications.
- **Neon in the Vercel Marketplace**: Neon is now a first-party native integration in the Vercel Marketplace. This integration lets Vercel users add Postgres to their projects and manage billing directly through Vercel. For details, see [Install the Neon Postgres Native Integration on Vercel](/docs/guides/vercel-native-integration).
- **Archive storage on the Free Plan**: Archive storage is now available on the Free Plan for automatically archiving inactive branches. This feature helps minimize storage costs, allowing us to expand the Free Plan even further. Learn more in [Branch Archiving](/docs/guides/branch-archiving).
- **Neon RLS**: This feature integrates with third-party **authentication providers** like Auth0, Clerk, and Stack Auth to bring authorization to your code base by leveraging Postgres [Row-Level Security (RLS)](https://www.postgresql.org/docs/current/ddl-rowsecurity.html). [Read the announcement](https://neon.tech/blog/introducing-neon-authorize) and [check out the docs](/docs/guides/neon-rls).
- **Neon on Azure**: You can deploy Neon databases on Azure, starting with the East US 2 region. This marks the first milestone on our Azure roadmap—many more exciting updates are on the way, including deeper integrations with the Azure ecosystem. [Read the announcement](https://neon.tech/blog/first-azure-region-available-in-neon).
- **End-to-end RAG pipelines in Postgres**: Our new and open source [pgrag](/docs/extensions/pgrag) extension lets you create end-to-end Retrieval-Augmented Generation (RAG) pipelines in Postgres. There's no need for additional programming languages or libraries. With the functions provided by `pgrag`, you can build a complete RAG pipeline directly within your SQL client.
- **Support for Analytics with pg_mooncake**: This new extension, brought to the community by [mooncake.dev](https://mooncake.dev/), introduces native columnstore tables with DuckDB execution for _fast_ analytics directly in Postgres. [Read the announcement](https://www.mooncake.dev/blog/pgmooncake-neon).
- **Datadog integration**: Scale and Business plan users can now export Neon metrics to Datadog.
- **Deletion of backup branches created by restore operations**: To help minimize storage and keep your Neon project organized, we added support for deleting obsolete backup branches created by [restore](/docs/guides/branch-restore) operations. Previously, these backup branches could not be removed. [Learn more](/docs/guides/branch-restore#deleting-backup-branches).
- **Read Replicas on the Free Plan**: Read Replicas are now available to all Neon users. [Read the announcement](https://neon.tech/blog/create-read-replicas-in-the-free-plan)
- **ISO27110 & ISO27701 compliance**: These new certifications add to our growing list of compliance achievements. For more about Neon's compliance milestones, see [Compliance](/docs/security/compliance).
- **Increased limits for Neon projects**: We increased the number of projects included in all our paid plans: Launch (100 projects), Scale (1000 projects), and Business (5000 projects). More projects supports use cases such as database-per-tenant and AI agents. [Read the announcement](https://neon.tech/blog/thousands-of-neon-projects-now-included-in-your-pricing-plan).
- **A new Postgres toolkit for AI agents and test environments**: We recently announced an experimental release of the [@neondatabase/toolkit](https://github.com/neondatabase/toolkit). This toolkit lets you spin up a Postgres database in seconds and run SQL queries. It includes both the [Neon API Client](https://www.npmjs.com/package/@neondatabase/api-client) and the [Neon Serverless Driver](https://github.com/neondatabase/serverless), making it an excellent choice for AI agents that need to quickly set up an SQL database, or for test environments where manually deploying a new database isn't practical. To learn more, see [Why we built @neondatabase/toolkit](https://neon.tech/blog/why-neondatabase-toolkit).
- **Postgres 17**: You can now run the very latest version of Postgres on Neon. [Read the announcement](https://neon.tech/blog/postgres-17).
- **SQL Editor AI features**: We added AI features to the Neon SQL Editor, including SQL generation, AI-generated query names, and an AI assistant that will fix your queries. [Learn more](/docs/get-started-with-neon/query-with-neon-sql-editor#ai-features).
- **A new Business plan with more compute and storage**: This new plan provides higher storage and compute allowances (500 GB-month storage and 1,000 compute hours) in addition to all of Neon's advanced features. It also offers potential cost savings for customers requiring more storage than our Scale plan provides. To learn more, please refer to our [Pricing](https://neon.tech/pricing) page and [Plans](/docs/introduction/plans) documentation.
- **Data migration support with inbound logical replication**: We've introduced inbound logical replication as the first step toward enabling seamless, low-downtime migrations from your current database provider to Neon. This feature allows you to use Neon as your development environment, taking advantage of developer-friendly tools like branching and our [GitHub integration](/docs/guides/neon-github-integration), even if you keep production with your existing provider. To get started, explore our guides for replicating data from AlloyDB, Aurora, CloudSQL, and RDS. See [Replicate data to Neon](/docs/guides/logical-replication-guide#replicate-data-to-neon). Inbound logical replication also supports migrating data between Neon projects, useful for version, region, or account migrations. See [Replicate data from one Neon project to another](/docs/guides/logical-replication-neon-to-neon).

</details>

For more of the latest features and fixes, check our [Changelog](/docs/changelog), published weekly. Or watch for our Changelog email, also sent out weekly. You can also subscribe to updates using our [RSS feed](/docs/changelog/rss.xml).

## Join the Neon Early Access Program

Help shape the future of Neon. Sign up for the **Early Access Program** and get:

- **Exclusive early access**: Get a first look at upcoming features before they go live
- **Private community**: Gain access to a dedicated Discord channel to connect with the Neon team and provide feedback to help shape what comes next
- **Weekly insights**: Receive updates on Neon's latest developments and future plans

The Early Access Program is available at two levels, which you can enable independently:

### Personal Early Access

Enable Early Access for your personal account to preview new features. Early Access features under this program level will only apply to projects under your personal account.

[Sign up now](https://console.neon.tech/app/settings/early-access) for your personal account to get started!

### Organization Early Access

Enable Early Access for your organization to preview new features. When an organization admin enables Early Access, everyone in your organization gets access to preview features across all projects belonging to that organization.

To enable Early Access for your organization, go to your organization **Settings** page in the Neon Console and **Join early access**.

If you need to opt out of Early Access later, [contact our Support team about Early Access changes](https://console.neon.tech/app/projects?modal=support) to ensure there's no disruption to features you may be using.

## A note about timing

We are as excited as you are to see new features in Neon, but their development, release, and timing are at our discretion.

## Share your thoughts

As always, we are listening. If you see something you like, something you disagree with, or something you'd love for us to add, let us know in our Discord feedback channel.

<CommunityBanner buttonText="Leave feedback" buttonUrl="https://discord.com/channels/1176467419317940276/1176788564890112042" logo="discord">Share your ideas in&nbsp;Discord</CommunityBanner>

## A brief history of Neon

The Neon **Limited Preview** started in February 2022 and was made available to a small number of select users and friends.

- On June 15th, 2022, the Neon team announced a [Technical Preview](https://neon.tech/blog/hello-world), making Neon available to a wider audience. Thousands of users were able to try Neon's [Free Plan](/docs/introduction/#free-plan).

- On December 6th, 2022, Neon released its branching feature and dropped the invite gate, welcoming everyone to try Neon's Free Plan.

- In the first quarter of 2023, Neon launched [paid plans](https://neon.tech/pricing) with new features like [Project Collaboration](/docs/guides/project-collaboration-guide), [Autoscaling](/docs/introduction/autoscaling), and [Scale to Zero](/docs/introduction/scale-to-zero). We also added support for AWS US East (N. Virginia)

- In the second quarter of 2023, we released the [Neon CLI](/docs/reference/neon-cli). Enhancements included a configurable [restore window](/docs/introduction/branch-restore) window, support for Postgres 16, and [SOC 2 Type 1](https://neon.tech/blog/soc2-type-1#our-journey-to-soc2) compliance.

- In the third quarter of 2023, we added [IP allowlisting](/docs/introduction/ip-allow), email signup, and [logical replication](/docs/introduction/logical-replication). We also announced [SOC 2 Type 2](https://neon.tech/blog/soc2-type2) compliance.

- In the fourth quarter of 2023, we added support for the AWS Asia Pacific (Sydney) region, [Instant restore](/docs/guides/branch-restore) with Time Travel Assist, and new [Pricing](https://neon.tech/pricing) plans.

- On April 15th, 2024, Neon announced [General Availability](https://neon.tech/blog/neon-ga).

For everything post-GA, please refer to our [Changelog](/docs/changelog) and the [Neon Blog](https://neon.tech/blog). You can also stay updated with the latest information and announcements by subscribing to our [RSS feeds](/docs/reference/feeds) or [newsletter](https://neon.tech/blog#subscribe-form).
