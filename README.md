# People-Directory
A simple web page that registers people (name & age) and stores the data
in a Supabase database. Each record can be toggled between two status
states (0 / 1) using a Toggle button.

Built with plain HTML, CSS, and JavaScript — no PHP or MySQL required.
Supabase replaces the traditional backend by exposing the database
directly through its JavaScript client.

# Features

- One-line form: Name, Age, Submit
- Data is inserted into a Supabase table (`users`)
- All records are displayed in a table below the form
- Each row has a Toggle button that switches its status between 0 and 1

# Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Database | Supabase (PostgreSQL) |
| Client library | @supabase/supabase-js (via CDN) |

# Setup Steps

# 1. Create a Supabase project
Created a project on [supabase.com](https://supabase.com) named
people-directory.

# 2. Create the database table
Ran the following SQL in the Supabase SQL Editor:
<img width="563" height="212" alt="image" src="https://github.com/user-attachments/assets/53e1a719-ea93-4081-becd-092be430d16c" />

# 3. Build the front-end
Created index.html containing:
- A form (Name, Age, Submit)
- A table (ID, Name, Age, Status, Action)
- A <script> that connects to Supabase using the URL and key above
- JavaScript functions to:
  - Insert a new record on Submit
  - Load and display all records
  - Toggle a record's status on button click

# 4. Test locally
<img width="700" height="252" alt="image" src="https://github.com/user-attachments/assets/f0f153e6-524c-4d5b-8540-3b2f9207b57f" />

# How to run

1. Clone this repository
2. Open index.html in any browser
3. Fill in Name and Age, click Submit
4. The table below updates automatically with all stored records
