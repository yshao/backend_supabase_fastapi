# Quick Start Guide

## Setup Environment Variables

1. Create your local environment file:
   cp .env.local.example .env.local

2. Edit .env.local and add your Supabase credentials from:
   https://app.supabase.com (Settings → API)

## Start Development

# Add pnpm to PATH (add to ~/.bashrc for persistence)
export PNPM_HOME="/home/yshao/.local/share/pnpm"
export PATH="$PNPM_HOME:$PATH"

# Activate Python virtual environment
source .venv/bin/activate

# Start all services
pnpm dev

This will start:
- Next.js frontend: http://localhost:3000
- FastAPI GraphQL API: http://localhost:8000
- GraphQL Playground: http://localhost:8000/graphql

## Available Commands

pnpm dev          # Start all services in development
pnpm build        # Build all packages and apps
pnpm lint         # Lint all TypeScript and Python code
pnpm lint:fix     # Fix linting issues automatically
pnpm test         # Run all tests (TypeScript and Python)
pnpm typecheck    # Run TypeScript and mypy type checking
pnpm clean        # Clean all build artifacts

## Project Structure

apps/web/         # Next.js React frontend
apps/api/         # FastAPI Python GraphQL API
.venv/            # Python virtual environment
docs/             # Project documentation

