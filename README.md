#!/bin/bash

echo "🚀 Preparing site for GitHub..."

# 1. Make sure we're on the main branch
git checkout main

# 2. Add all changes
echo "📁 Staging files..."
git add .

# 3. Commit with auto‑message
echo "📝 Committing..."
git commit -m "Deploy: updated site build"

# 4. Push to GitHub
echo "📤 Pushing to GitHub..."
git push origin main

echo "✅ Deployment complete!"
