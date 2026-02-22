# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the documentation repository for Rise Gaming's Takistan Life Arma 3 gamemode, containing marketing materials, player guides, and feature documentation for a 6-faction roleplay server.

## Repository Structure

- `README.md` - Main repository description
- `docs/player-guides/USER_GUIDE.md` - Complete player guide with controls, economy, factions, and gameplay mechanics
- `docs/technical/FEATURE_MAP.md` - Comprehensive feature overview with matrices and analysis
- `docs/marketing/AD_BRIEFS.md` - Marketing materials and promotional content
- `docs/technical/feature_catalog.json` - Detailed JSON catalog of 28+ game features with code references

## Content Guidelines

This repository contains defensive documentation for game security and player education. All content is designed to:
- Help players understand game mechanics legally
- Document existing features for player reference  
- Provide marketing materials for server promotion
- Catalog functionality for maintenance and updates

## Document Types

### Player Documentation
- `docs/player-guides/USER_GUIDE.md` - Contains comprehensive gameplay instructions, faction abilities, economy guides, and control references
- Content is educational and focuses on legitimate gameplay mechanics

### Technical Documentation  
- `docs/technical/feature_catalog.json` - Contains structured data about game features including:
  - Code file references with line numbers and commit SHAs
  - Feature categories, dependencies, and test procedures
  - Economic data, legal status, and game balance information

### Marketing Materials
- `docs/marketing/AD_BRIEFS.md` - Promotional content highlighting server features
- `docs/technical/FEATURE_MAP.md` - Strategic overview for potential players

## Key Feature Areas Documented

1. **Economy System** - Legal mining, illegal drug processing, factory production, banking
2. **Law Enforcement** - Arrest mechanics, prison system, crime categories, bail system  
3. **Faction Warfare** - 6 distinct factions with unique abilities and restrictions
4. **Territory Control** - 27 capturable zones, gang territories, war mechanics
5. **Government** - Elections, leadership powers, democracy vs dictatorship gameplay
6. **Medical System** - ESU revival mechanics, death timers, organ harvesting
7. **Vehicle Management** - Ownership, garages, upgrades, sharing systems

## Working with This Repository

When editing documentation:
- Maintain accuracy with referenced code base (commit 33b1595)
- Update cross-references between documents when changing feature descriptions
- Preserve marketing tone in docs/marketing/AD_BRIEFS.md while keeping technical accuracy
- Update feature counts and statistics in docs/technical/FEATURE_MAP.md when adding new features
- Maintain JSON structure integrity in docs/technical/feature_catalog.json

## Code References

All documentation references the actual Rise Gaming Takistan Life Arma 3 codebase. Code citations include:
- File paths relative to game mission root
- Specific line numbers where features are implemented  
- Commit SHA (33b1595) for version tracking
- Functional reasoning for why code sections are referenced

This documentation serves as both player education and development reference for the live Arma 3 server implementation.