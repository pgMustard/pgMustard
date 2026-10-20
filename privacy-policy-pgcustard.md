# pgCustard privacy policy

pgCustard is made by pgMustard Ltd, a UK company.

When you use hosted pgCustard (app.pgcustard.com), we collect, store, and use the personal information below. Running pgCustard yourself is [covered at the end](#self-hosted).

### Email address

We need this to email you about your databases. When you sign in with Google or GitHub, they tell us your email address and an account ID, which we use to recognise you. We store both in our database (hosted in Finland), but not your name or a password.

If you email us or book a call, your details will also be in Google Workspace and SavvyCal respectively.

### Database connection details

We need these to collect metrics from your databases: the host, port, database name, username, password, and CA certificate, plus any details you give us for reading host metrics from your cloud provider. Passwords and keys are encrypted with a separate key for each organisation, which is in turn protected by Google Cloud’s Key Management Service.

### Metrics

Every 30 seconds we read Postgres’s statistics views and catalogs: things like schema, table, and index names, sizes, settings, and activity counts, plus normalised query text from `pg_stat_statements`. We ask you to connect us with a role that has `pg_monitor`, which can read statistics but not the data in your tables.

Metrics are processed under our [data processing agreement](https://pgcustard.com/dpa), and stored in our database in the Google Cloud data centre in Finland. Most are kept for around 100 days, and table events (such as vacuums) for 400 days. Query text, weekly summaries, and alerts are kept until you remove the database.

### Emails

We email weekly summaries and alerts to members of your organisation, sent through Mailchimp Transactional. These contain similar information to the app, such as object names and normalised query text. We don’t track whether emails are opened or links clicked.

### Payments

We use Stripe to take payments. When you subscribe, they collect your card details, billing address, and your VAT number if you give one. We pass them your organisation’s name and your email address, and we never see your card number.

### Technical information

To serve web requests, Google Cloud records technical information such as your IP address and browser agent. Our logs also record errors, which can include your database’s host name, for example when we can’t reach it. Logs are deleted after 30 days.

We use two cookies: one to keep you signed in, for 30 days, and one that lasts ten minutes while you sign in. We don’t use analytics or tracking cookies. Our website, pgcustard.com, is hosted by Cloudflare and uses Fathom Analytics, which doesn’t use cookies. Both also process your IP address and browser agent.

### If you leave

After you cancel your pgCustard subscription, we’ll keep everything for 7 days, just in case. Within a week after that, we’ll delete your data and your account, keeping only what we need to hold a record of the service we provided to you. If you’d like us to delete anything sooner, just ask.

### Self-hosted

If you run pgCustard yourself, your metrics stay in your own database and are never sent to us. To let your server download new versions from our image registry (Google Artifact Registry), we give you a key named after your company. Google sees these downloads, including the IP address they come from, but we don’t log them.

### Your rights

We use this information to provide pgCustard and keep it secure. Most of the services named here process it in other countries, all with appropriate safeguards in place. We don’t sell your information or share it beyond these services, except as required by law.

If you’re unhappy with how we handle your information, please tell us, and we’ll do our best to put it right. You can also contact your local data protection authority.

You can ask us for a copy of your personal information, or ask us to correct or delete it, by emailing hello@pgmustard.com.

_The effective date of this policy, as well as its history, can be viewed by pressing the "history" button at the top_
