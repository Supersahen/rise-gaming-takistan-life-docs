# Rise Gaming Takistan Life — Feature Map

**Repository:** git@github.com:RiseGaming/Rise-Gaming-Takistan-Life.git  
**Commit:** 33b1595 | **Date:** 2025-08-25

## Feature Categories Overview

| Category | Feature Count | Faction Access | Risk Level |
|----------|--------------|----------------|------------|
| Economy | 8 | All | Mixed |
| Law Enforcement | 7 | Police/OPFOR | Legal |
| Combat & Territory | 4 | Police/TLA | Legal |
| Medical | 1 | Police/TLA | Legal |
| Vehicles | 2 | All | Legal |
| Gangs | 2 | Civilian | Legal |
| Entertainment | 2 | All | Legal |
| Jobs | 2 | Police/TLA/Indies/Civs | Mixed |
| Government | 3 | Leadership | Legal |
| Licenses | 2 | All | Legal |

## Economy Features Matrix

| Feature | Legal | Profit Range | License Required | Time Investment | Location Type |
|---------|-------|--------------|------------------|-----------------|---------------|
| Mine Copper Ore | ✅ | $1,500/unit | Mining Tool | Low | Mining Site |
| Process Copper | ✅ | $4,000/unit | Mining License ($100k) | Medium | Refinery |
| Harvest Marijuana | ❌ | $80/unit | None | Low | Drug Field |
| Process Marijuana | ❌ | $14,000/unit | Processing ($17k) | Medium | Drug Lab |
| ATM Banking | ✅ | Interest | None | Instant | ATM/Mobile |
| Factory Production | ✅ | 30% savings | None | High | Factory |
| Crate Delivery | Mixed | $100-250k | None | 20 min | Spawn→Delivery |
| VIP Pass Benefits | ✅ | 2x interest | VIP ($50M) | Instant | Premium |

## Law Enforcement System

| Feature | Authority | Target | Penalty | Equipment | Range/Limit |
|---------|-----------|--------|---------|-----------|-------------|
| Arrest Criminal | Police/OPFOR | Wanted Players | Jail+Bail | Restraints | 50-75m to prison |
| Prison System | Automatic | Arrested | 2-20 min | Uniform | Escape at 75m |
| Pay Bail | Prisoner | Self | $150k-1M | Money | Hospital |
| Speed Radar | Police | Vehicles | Tickets | Radar Gun | 100m |
| Spike Strips | Police/OPFOR | Vehicles | Tire damage | Item | Contact |
| Vehicle Impound | Police/OPFOR | Illegal parking | Storage fee | Authority | Direct |
| Ticket System | Police/OPFOR | Minor crimes | Fines | Authority | Direct |

## Territory Control System

| Territory Type | Capture Time | Controllers | Peacetime Rules | Rewards |
|---------------|--------------|-------------|-----------------|---------|
| North Territories (12) | 30 seconds | Police/OPFOR | Police only | 1 rank point |
| South Territories (15) | 30 seconds | Police/OPFOR | OPFOR only | 1 rank point |
| Gang Areas (3) | 60 seconds | Gang members | Always open | Gang control |
| Safe Zones | N/A | System | No combat | Protection |

## Faction Capabilities

| Faction | Slots | Can Arrest | Can Process Drugs | Can Declare War | Can Revive | Special Equipment |
|---------|-------|------------|------------------|-----------------|------------|-------------------|
| Civilian | 64 | ❌ | ✅ | ❌ | ❌ | Gang access |
| Police/NATO | 22 | ✅ | ❌ | ❌ | ❌ | Radar, spikes |
| Insurgent | 11 | ❌ | ✅ | ❌ | ❌ | Explosives |
| OPFOR/TLA | 22 | ✅ | ❌ | ✅ | ❌ | Military gear |
| ESU/Medical | 10 | ❌ | ❌ | ❌ | ✅ | Medical equipment |
| PMC | 5 | ❌ | ✅ | ❌ | ❌ | Contract access |

## Vehicle & Transportation

| System | Cost | Storage | Features | Restrictions |
|--------|------|---------|----------|--------------|
| Garage Storage | $1,000/vehicle | Persistent | Store/Retrieve/Sell | Faction garages |
| Vehicle Purchase | Variable | Keys issued | Ownership | License required |
| Vehicle Upgrades | $75-100k | Permanent | Nitro/Speed | Modification shops |
| Vehicle Keys | Free | Shareable | Lock/Unlock | Owner control |

## Criminal Justice Pipeline

```
CRIME COMMITTED → WANTED STATUS → POLICE PURSUIT → ARREST
                                          ↓
                              PRISON (2-20 min) ← CHARGES ASSIGNED
                                          ↓
                              PAY BAIL or SERVE TIME → RELEASE
```

## Economic Flow Chart

```
LEGAL PATH:
Mine Raw → Process (License) → Sell Refined → $4-18k profit

ILLEGAL PATH:
Harvest Drugs → Process (License) → Sell Product → $14-175k profit
                                            ↓
                                    RISK: Arrest/Seizure

JOB PATH:
Accept Delivery → Transport Crate → Complete in 20min → $100-250k
```

## License Progression

| Tier | License Type | Cost Range | Unlocks |
|------|-------------|------------|---------|
| Basic | Driver, Pistol | $5-50k | Basic operations |
| Professional | Mining, Processing | $17-100k | Economic activities |
| Advanced | Automatic, Pilot | $300-500k | Heavy equipment |
| Elite | Arms Dealer | $10M | Premium shops |
| Ultimate | VIP Pass | $50M | All benefits |

## Map Zones

| Zone Type | Marker Examples | Purpose | Access |
|-----------|----------------|---------|--------|
| Spawn Points | cop_base_spawn, prisonspawn | Faction starts | Faction only |
| Economic | takistan_mine_1, refinery_1 | Resource processing | Licensed |
| Commercial | carshop1, gunshop1 | Shopping | Money required |
| Criminal | drug_field, black_market | Illegal activities | Restricted |
| Government | dmv, university, voting_booth | Services | Public |
| Entertainment | casino | Games | Age restricted |
| Strategic | gangarea1, territory flags | Control points | Contested |

## Communication & UI Access Points

| Interface | Access Method | Primary Function | Availability |
|-----------|--------------|------------------|--------------|
| Interaction Menu | Windows Key | Player/Object actions | Always |
| ATM Dialog | Near ATM or Mobile App | Banking | Location/App |
| Garage Dialog | At garage markers | Vehicle management | Garages |
| Shop Dialog | At shop NPCs | Buy/Sell items | Shops |
| Factory Dialog | At factories | Manufacturing | Factories |
| Gang Menu | Gang system | Gang management | Gang members |
| Death Screen | On death | Respawn options | When dead |
| Election Dialog | Voting booths | Cast votes | Election period |

## Risk vs Reward Analysis

| Activity | Risk Level | Potential Profit | Time to Profit | Startup Cost |
|----------|------------|------------------|----------------|--------------|
| Mining | None | $18k/batch | 10 min | $102k |
| Drug Processing | Very High | $175k/batch | 15 min | $17-50k |
| Crate Delivery | Low-Medium | $100-250k | 20 min | None |
| Factory Work | None | 30% savings | Variable | Item cost |
| Gang Territory | Medium | Control benefits | 60 sec | $500k gang |
| Casino | Financial | Up to 35x bet | Instant | Bet amount |

## Persistence & Saves

| Data Type | Storage | Save Trigger | Faction Specific |
|-----------|---------|--------------|------------------|
| Bank Balance | ServerDB | On transaction | No |
| Inventory | ServerDB | On change | No |
| Licenses | ServerDB | On purchase | No |
| Vehicle Ownership | ServerDB | On buy/sell | No |
| Gang Membership | ServerDB | On join/leave | No |
| Jail Status | ServerDB | On arrest/release | No |
| Territory Control | Mission | On capture | Yes |
| Election Results | Server | On vote end | Yes |

## Feature Dependencies

```
Economy System
    ├── License System (enables processing)
    ├── Shop System (buy/sell interface)
    ├── Banking System (money storage)
    └── Factory System (production)

Law System
    ├── Arrest System (capture criminals)
    ├── Prison System (serve time)
    ├── Warrant System (track crimes)
    └── Bounty System (rewards)

Combat System
    ├── Territory Capture (control zones)
    ├── Gang Warfare (group combat)
    ├── War Declaration (faction war)
    └── Bomb System (terror tools)
```

## Key Statistics

- **Total Features Documented:** 28 major systems
- **Faction-Exclusive Features:** 12
- **License-Gated Features:** 15
- **Illegal Activities:** 8
- **Legal Activities:** 20
- **Maximum Jail Time:** 20 minutes
- **Maximum Bail:** $1,000,000
- **Highest Legal Profit:** $18,000/unit (Platinum)
- **Highest Illegal Profit:** $175,000/unit (Meth)
- **Total Capturable Territories:** 30 (27 faction + 3 gang)