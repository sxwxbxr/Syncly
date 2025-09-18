# Syncly
Ein Multi Kalender Sync fuer Google Microsoft und iCal mit Konflikt Erkennung.

## Ziel
Termine bidirektional synchronisieren Dubletten verhindern und Regeln anwenden.

## Features
* Verknuepfung mehrerer Accounts
* Regeln fuer Sichtbarkeit und Kategorien
* Konflikt Erkennung
* Trockentest Modus

## Tech Stack
* Python FastAPI
* APScheduler fuer Jobs
* Postgres
* Microsoft Graph API
* Google Calendar API
* OAuth PKCE

## Kritische Packages
* fastapi httpx
* apscheduler
* authlib
* google api python client
* msal
* sqlalchemy alembic

## Env Variablen
* GOOGLE_CLIENT_ID
* GOOGLE_CLIENT_SECRET
* MS_CLIENT_ID
* MS_CLIENT_SECRET
* OAUTH_REDIRECT_URI
* DATABASE_URL

## Datenmodell
* account calendar sync rule event map job log

## Setup
* alembic upgrade head
* uvicorn main

## Tests
* Fake Provider und Mapping Tests

## CI
* Contract Tests gegen Sandbox Kalender

## Security
* Least Scope
* Token Verschluesselung at rest

## Roadmap
* ICS Export Server
* Team Richtlinien

## Lizenz
AGPL
