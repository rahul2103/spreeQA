# SpreeQA


## Prerequisites

Before you begin, make sure you have the following prerequisites installed on your system:

- Ruby 3.3.0
- Rails 7.1.3.4
- Postgresql 14.11

## Installation

1. **Clone the project** using the provided URL:

   ```bash
   git clone https://github.com/AasPass-Marketplace/spree480.git
   ```

2. **Install the required gems** using Bundler:

    ```bash
    bundle config set --local path .gemfiles

    bundle install
    ```

    Or, you can use:

    ```bash
    bundle install --path .gemfiles
    ```

3. Create a **```database.yml```** file and configure your database settings. You can refer to the **```config/database.yml.example```** file for reference.

4. **Create the database:**

    ```bash
    RAILS_ENV=development bundle exec rails db:create
    ```

5. **Run database migrations:**

   ```bash
   RAILS_ENV=development bundle exec rails db:migrate
   ```

6. **Add app credentials:**

   - **config/master.key** ```abc```

6. **Seed the database:**

   ```ruby
   bundle exec rails db:seed
   ```
7. **Compile assets for development:**

   ```bash
   RAILS_ENV=development bundle exec rails assets:clean assets:precompile
   ```
8. **Restart your server.**

   If it was already running, make sure to restart it so that it can find the assets properly.
