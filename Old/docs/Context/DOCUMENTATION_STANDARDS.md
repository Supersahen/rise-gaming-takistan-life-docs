# Documentation Standards - Rise Gaming Takistan Life Player Guides

This document captures the authorial guidelines and factual constraints for maintaining accuracy and consistency across Takistan Life player documentation. All future updates should adhere to these standards.

## Language and Tone

- Use professional, clear language suitable for new players unfamiliar with the server.
- Avoid internal jargon, function names, code markers, or developer identifiers.
- Do not use terms like "gotchas" or informal language; instead use professional alternatives such as "operational notes," "practical considerations," or "key points to remember."
- Avoid repetitive clarification; if something is false, omit it entirely rather than stating what it is not. For example:
  - ✗ Bad: "Drugs cannot be sold through a generic black market interface."
  - ✓ Good: (omit entirely; simply state where drugs are sold)
  - ✗ Bad: "Mining increases risk and does not change yield or processing time."
  - ✓ Good: "Mining during high-player periods carries increased risk of robbery or kidnapping as popular mining areas attract criminals."

## Map Markers and Locations

- Do not use internal map marker variable names (e.g., `takistan_mine_1`, `prisonspawn_opf`, `refinery_1`).
- Use player-friendly location descriptions: "Resource Refinery," "police headquarters," "civilian spawn," "northern VIP location south of Rasman," etc.
- When internal marker names are unavailable, describe the location by geography, nearby towns, or nearby structures (e.g., "impound lot on the north airfield near police base").

## Licensing and Training Names

- Use friendly, in-game licence names rather than technical identifiers:
  - ✗ Bad: `paramedic_license`, `jihadi_training`, `pmc_license_journeyman`
  - ✓ Good: ESU Training, Jihadi Training (friendly name), PMC Journeyman License
- When referring to a licence, use the full in-game name as shown in-game:
  - Example: "Purchase the Mining License at the civilian licensing shop to enable ore processing."

## Licensed Locations and Shop Names

- Civilian licensing basic licenses: sold at the **Civilian Licensing Shop** (at civilian spawn).
- Weapons and professional licenses: sold at the **Weapons Licensing Store** south of Rasman and the **Full License Store** near the airfields (sells passports, pilot licenses, truck certifications, engineer licenses).
- Arms Dealers: **Western Arms Dealer** (north) and **Eastern Arms Dealer** (south) — each requires a $10,000,000 license purchase to access. List the categories of equipment available at each.
- Farmers Market: sells sickles, hoes, and legal crops; is the purchasing point for legal crops (apples, tobacco, cotton, oranges, wheat).
- Bus Depot & Tow Truck Depot: located at the impound lot south of Rasman (same location as VIP location). Civilians may become bus drivers or tow drivers here.

## Inventory and Item Usage

- Items are used via the inventory menu: "Open your inventory, select the item, and choose use."
- Do not mention "quick-access slots" or similar non-existent mechanics.
- Private storage is for virtual inventory items (spike strips, bank insurance, ores, crops, drugs, etc.); guns and ammunition are Arma 3 items and cannot be stored in private storage.
- All factions have private storage at their spawn location; for civilians this is marked as "DMV - Private Storage" at their spawn.

## Factions and Roles

### Police / BLUFOR
- Abbreviated as "Police" or "BLUFOR."
- Cannot access war vehicles outside declared war or martial law; vehicles must be returned to base or stored when war/martial law ends.
- Drones: can operate military reconnaissance and (during war/martial law) armed drones. **Cannot send drones into the south.**
- SRT (Special Response Team): whitelisted elite unit applying via the application channel. Located in a secured area adjacent to police HQ; operates within same baseline systems as police.
- Spike strips, weapon/item bags, defusers, tracking chips, bait car kits: all available and detailed in the Police guide.

### OPFOR / TLA
- Abbreviated as "OPFOR" or "TLA."
- Cannot access war vehicles outside declared war; vehicles must be returned to base or stored when war ends.
- Can send drones into the north. Cannot maintain drone presence in the south during peace.
- OSF (OPFOR Special Forces): whitelisted equivalent of SRT, applying via application channel. Treated with higher regard, expanded gear access. OSF can make interdictions into the north with RP justification during war; BLUFOR can shoot or arrest them on site.
- Commander: final authority on large-scale operations; controls southern tax rates.

### Civilians
- Can garage vehicles at their spawn point (10% fee on vehicle price; 10k additional if impounded).
- Can become bus drivers or tow truck drivers at the bus/tow depot (impound lot south of Rasman).
- Can purchase access to Western Arms Dealer ($10M license) to access militarised weapons.
- Can harvest legal crops (apples, tobacco, cotton, oranges, wheat) and sell back at Farmers Market.
- Can access chop shops (Nur in the north; south of the border near Falar and Anar) to sell vehicles they may not own (reduced payout, illegal).
- Can use Contracting App to request PMC protection during risky activities (mining, drug runs).
- Private storage location: "DMV - Private Storage" at civilian spawn.

### Police & OPFOR (Vehicle Impounding)
- Garage fees: 15% of vehicle price (10% additional if impounded).
- Impound locations: north airfield near police base, south airfield near OPFOR base, northern VIP location south of Rasman.
- Tow mechanics: when police impound a vehicle, a request is sent to active tow truck drivers (civilian role). Tow driver must collect the vehicle with their tow truck. Without an active tow driver, the vehicle is lost.

### Insurgents
- Cannot create or join civilian gangs; operate via faction networks.
- Can access chop shops (same as civilians).
- Can request bombing missions at an ATM (requester receives bomb, is responsible for planting and defending; mission fails if requester dies).
- Drones: can purchase reconnaissance and bomb-dropping drones (controlled via UAV terminal).
- Supply convoy mechanic: insurgents must return captured supply convoys to their base to increase restricted weapon/vehicle supply.

### ESU
- Must remain neutral and impartial; cannot take sides in faction conflicts.
- Cannot revive players in active firefights or contested areas unless both parties permit.
- Shares banking system with civilians.

### PMC
- Whitelisted and requires application via the application channel.
- Maintains inventory on death (does not lose items).
- Can be contracted by civilians and other factions for protection, escort, and contract work.
- Can create contracts via Contracting App for protection services.

## Specific Systems

### Convoys
Three separate convoys spawn on 45-minute intervals (not simultaneously; timing is fixed at 45 minutes between spawns, start time varies):
- BLUFOR Government Convoy: must take back to BLUFOR base. Civilians and insurgents can rob it.
- OPFOR Government Convoy: must take back to OPFOR base. Civilians and insurgents can rob it.
- Insurgent Supply Convoy: must take back to insurgent base to increase restricted weapon/vehicle supply.
- War interdictions: BLUFOR and OPFOR can rob each other's convoy during declared war. OSF can interdict the convoy into the north with RP justification; BLUFOR can shoot or arrest OSF on site.

### Bank Insurance
- Money held in faction bank is lost on death unless the player has bank insurance.
- Exception: VIP players do not need bank insurance; their bank is protected automatically.
- Bank insurance is a purchasable virtual inventory item available at spawn.

### Garage System
- All factions can garage vehicles at their spawn to store them persistently.
- Garage fee: 10% of vehicle price for civilians, independents, and non-police. Police and OPFOR: 15% of vehicle price.
- Impounded vehicles: additional +$10,000 flat fee on top of normal garage fee. Retrieved from impound lots (not faction spawn).
- Impound locations: north airfield near police base, south airfield near OPFOR base, Rasman area (northern VIP location south of Rasman).

### Drones & UAV Terminals
- UAV terminals are expensive and must be purchased.
- BLUFOR and OPFOR maintain inventory on death, making UAV purchase easier for them.
- Insurgents and civilians lose UAV terminals on death (high-risk purchase).
- Drone types and restrictions:
  - Insurgents: bomb-dropping drones and reconnaissance drones.
  - BLUFOR/OPFOR: military reconnaissance drones. BLUFOR can also use armed drones (Predators) during war or martial law.
  - BLUFOR: **cannot send drones into the south.**
  - OPFOR: **can send drones into the north.**
  - Civilians: basic drones with limited camera functionality.

### Gas Stations
All factions have access. Gas stations provide:
- Refuelling for low-fuel vehicles.
- Purchase items: jerry cans, medikits, earplugs, energy drinks, repair kits, knife (organ harvesting), siphon fuel kit (fuel theft; suspicious but not necessarily illegal), lighter (vehicle ignition; suspicious but not necessarily illegal).

### General Player Tips (All Factions)
- Night Vision: purchasable at all spawn points. The server has a day/night cycle; nights are pitch-black outside populated areas. Night vision is recommended.
- Repair Kits & Refuel Kits: carry these to prevent becoming stranded. Available at gas stations and spawn points.
- Medikits: purchase from gas stations and most spawn points; heals most injuries. ESU can provide full healing.
- Energy Drinks: available at many locations; increases sprint distance.
- Steroids: legal and illegal versions available at pharmacies; temporarily increase inventory space (useful for mining or bulk hauling).
- Earplugs: purchasable at spawn points; equip via Home key (default). Protect against hearing-based effects.
- Vehicle Ammo: purchasable at various locations; rearmed armed vehicles when used from inside the vehicle.
- Speed Upgrades & Nitro Kits: available at car shops and spawn points. Speed upgrades increase max speed; Nitro adds a speed boost (press Q) at high fuel cost. Benefits vary by vehicle (some gain significant boosts, others minor increases).
- Gas Masks: purchasable at most clothing shops. Essential for BLUFOR and OPFOR (tear gas protection); accessible to civilians and independents as well.
- Contracting App: civilians can request protection via this app if PMC is active. PMC will likely reach out to discuss contract terms.

### Legal Crop Harvesting (Civilians)
- Legal crops: apples, tobacco, cotton, oranges, wheat.
- Harvest locations: yellow circles marked on the map throughout the world.
- Tools: sickle or hoe (purchased from Farmers Market).
- Returns: lower profit than illegal drugs but safe and legal.
- Sale location: sell back to Farmers Market.

### Chop Shops (Civilians & Insurgents)
- Locations: Nur (north); south of the border near Falar and Anar.
- Function: sell vehicles that may not belong to the seller for a reduced payout (illegal activity).

### Weapons Licenses and Restrictions
- Illegal weapons: civilians and insurgents must purchase weapons licenses or use black-market sources.
- Legal weapons: police and military factions have access to weapons from faction shops.

## Meth Production
- Precursors are purchased from pharmacies in major towns.
- Processing occurs at a single meth lab in the far north-west of the map (near Nur and Nagara).
- Meth production may result in explosions during processing. Do not detail the mixing process separately.
- Risk and reward are appropriate for guides; legal penalties are severe.

## Scythe vs. Hoe
- All references to "scythe" should use "hoe" instead.
- Both sickles and hoes are tools used for harvesting legal crops and raw plant drugs.

## Bombing Missions (Insurgents)
- Can be requested (not required) at an ATM.
- The requesting player receives the bomb and is responsible for planting and defending it.
- Mission fails if the requester dies before planting or if conditions are not met.

## Tow Truck Mechanic
- When police impound a vehicle, the system sends a request to active tow truck drivers (civilian role).
- Tow driver must use their tow truck to collect and haul the vehicle to impound.
- Without an active tow driver, the impounded vehicle is lost (disappears).

## Armour Requirements and Rank Progression
- Police rank system gates access to armoury crates and equipment tiers.
- Other factions (OPFOR, insurgents, ESU) have rank systems primarily for RP and status.
- SRT and OSF are able to bypass normal rank restrictions due to special unit status.

## No Statements About Non-Existence
- Do not include clarifying statements about what doesn't exist or isn't possible unless directly relevant to avoiding player confusion.
- Example: If drugs cannot be sold at a black market, do not mention a "black market interface" at all. Simply state where drugs are sold.

## Cross-Document Linking
- Guides should reference each other where relevant.
- The main USER_GUIDE.md should summarise key mechanics and link to faction-specific guides.
- A generic tips guide (all-factions) should be created for universally applicable mechanics.

## Last Updated Footer
- Do **not** include "Last updated" footers or timestamps in guides. They are reference documents, not official announcements.

---

*This standards document should be referenced when updating or creating new guides to ensure consistency and player clarity.*
