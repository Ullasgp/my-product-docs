Step-by-Step Guide to Learn Redocly Documentation

(For Technical Writers & Beginners)

What is Redocly?

Redocly Official Website

Redocly is a tool used to:

Create beautiful API documentation
Convert OpenAPI/Swagger files into professional docs
Publish API portals
Validate API specifications
Maintain Docs-as-Code workflow

It is widely used in banking, fintech, SaaS, and enterprise projects.

Understanding the Complete Flow
Backend Team Creates APIs
        ↓
Swagger/OpenAPI JSON or YAML File
        ↓
Redocly Reads the File
        ↓
Beautiful API Documentation Generated
        ↓
Publish to Internal/External Users
Prerequisites

Before learning Redocly, you should know:

Requirement	Why Needed
Basic command line	To run commands
Git basics	Docs-as-code workflow
YAML basics	OpenAPI files are written in YAML
Swagger/OpenAPI basics	Redocly works on OpenAPI specs
VS Code	Editing files
STEP 1 — Install VS Code

Download:

Visual Studio Code

Installation
Open website
Download for:
Mac
Windows
Install normally
STEP 2 — Install Node.js

Redocly CLI works using Node.js.

Download:

Node.js Official Website

Install:

Choose LTS version
Next → Next → Install
STEP 3 — Verify Installation

Open Terminal (Mac) or Command Prompt (Windows).

Run:

node -v

Example output:

v22.1.0

Now check npm:

npm -v

Example:

10.5.0
STEP 4 — Install Redocly CLI

Open terminal.

Run:

npm install -g @redocly/cli
STEP 5 — Verify Redocly Installation

Run:

redocly --version

Example:

2.0.0
STEP 6 — Create Project Folder

Move to Desktop:

cd Desktop

Create folder:

mkdir redocly-project

Go inside folder:

cd redocly-project
STEP 7 — Open Folder in VS Code

Run:

code .

If code command not working:

Mac Fix

Open VS Code:

Press Cmd + Shift + P
Type:
Shell Command: Install 'code' command in PATH
Click it
Restart terminal

Now again run:

code .
STEP 8 — Create OpenAPI File

Create file:

openapi.yaml
STEP 9 — Add Sample API Specification

Paste this content:

openapi: 3.0.0

info:
  title: User API
  version: 1.0.0
  description: Sample API documentation using Redocly

servers:
  - url: https://api.example.com

paths:
  /users:
    get:
      summary: Get User List
      description: Returns all users
      responses:
        '200':
          description: Successful response

Save file.

STEP 10 — Preview Documentation
