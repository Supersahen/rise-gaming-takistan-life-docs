# Technical Documentation

This directory contains technical documentation, feature specifications, and structured data designed for developers, administrators, and automated content generation systems.

## Contents

### [FEATURE_MAP.md](FEATURE_MAP.md)
Strategic feature overview with analysis matrices showing:
- Feature categorization and relationships
- System dependencies and interactions  
- Implementation complexity and status
- Player impact and usage patterns

### [feature_catalog.json](feature_catalog.json) 🤖
**LLM-Optimized Feature Database** containing structured data for 28+ game features with:
- Complete feature specifications with code references
- Economic data, legal status, and game balance information
- UI/UX details, controls, and player interaction methods
- Persistence, networking, and technical implementation details

## 🤖 LLM Integration Guide

The `feature_catalog.json` file is specifically designed for Large Language Model (LLM) integration to automatically generate documentation, marketing materials, and player guides.

### Data Structure
Each feature entry contains standardized fields optimized for AI processing:
```json
{
  "id": "unique-feature-identifier",
  "name": "Human Readable Name",
  "category": "economy|law|combat|government|medical|etc",
  "roles": ["civilian", "police", "rebel", "opfor", "esu", "pmc"],
  "summary": "Concise description for AI understanding",
  "how_to_access": {
    "triggers": ["User actions required"],
    "preconditions": ["Requirements that must be met"]
  },
  "controls_ui": {
    "dialogs": ["UI dialog names"],
    "notifications": ["Player feedback messages"],
    "keybinds": ["Control inputs"]
  },
  "locations_markers": ["Map locations where feature is available"],
  "economy_law": {
    "costs": [{"type": "item", "amount": 1000, "currency": "$"}],
    "payouts": [{"activity": "action", "amount": 2000}],
    "illegality": "legal|illegal|mixed",
    "penalties": ["Consequences for illegal activities"]
  },
  "code_refs": [
    {
      "path": "file/path.sqf",
      "lines": "L100-150",
      "sha": "33b1595",
      "reason": "Why this code is referenced"
    }
  ],
  "confidence": 0.95
}
```

### LLM Prompt Examples

#### Generate Player Tutorial
```
Create a step-by-step tutorial for new players explaining how to use the mining system in Takistan Life. Use the feature data from feature_catalog.json for accurate information about costs, locations, and procedures. Include specific keybinds and expected outcomes.

Reference features: mine-copper-ore, process-copper-refinery
```

#### Create Marketing Content  
```
Write an exciting promotional description highlighting the criminal underworld features in Takistan Life. Focus on the risk/reward mechanics and role-playing opportunities. Base content on the drug processing and gang territory features from feature_catalog.json.

Reference features: harvest-marijuana, process-marijuana, gang-create, gang-capture-area
```

#### Generate Technical Documentation
```
Create API documentation for the arrest system explaining the technical implementation, networking requirements, and integration points. Use the code references and technical details from feature_catalog.json.

Reference features: arrest-criminal, jail-time-system, pay-bail
```

#### Faction-Specific Guide Generation
```
Generate a comprehensive guide for new police officers explaining all law enforcement features, tools, and procedures. Include economic incentives, required equipment, and interaction methods. Extract relevant information from all police-role features in feature_catalog.json.

Filter by: "roles": ["police"]
```

#### Economic Analysis Report
```
Analyze the economic balance of all money-making activities in Takistan Life. Create a profitability comparison table including risk factors, time investment, and legal status. Use economic data from all features in feature_catalog.json.

Focus on: economy_law.payouts, economy_law.costs, economy_law.illegality
```

### Advanced LLM Usage Patterns

#### Content Generation Pipeline
1. **Query Features**: Filter feature_catalog.json by category, role, or tags
2. **Extract Data**: Pull relevant fields for specific content type
3. **Generate Content**: Use structured prompts with feature specifications
4. **Cross-Reference**: Validate against code_refs and confidence scores
5. **Format Output**: Apply appropriate styling for target medium

#### Multi-Feature Synthesis
```
Create a comprehensive "Day in the Life" scenario showing how a civilian player might interact with multiple game systems. Use feature dependencies and locations to create a realistic progression through mining, processing, trading, and banking activities.

Chain features: mine-copper-ore → process-copper-refinery → atm-banking → vehicle-garage
```

#### Dynamic Updates
```
When feature_catalog.json is updated, automatically regenerate all affected documentation sections. Compare confidence scores and code_refs to identify features that may have changed implementations.
```

### API-Style Queries

The JSON structure supports complex queries for automated processing:
```javascript
// Find all illegal activities with high payouts
const highValueCrime = features.filter(f => 
  f.economy_law.illegality === "illegal" && 
  f.economy_law.payouts.some(p => p.amount > 10000)
);

// Get all features available to new players
const civilianFeatures = features.filter(f => 
  f.roles.includes("civilian") && 
  f.confidence > 0.9
);

// Generate location-based content
const locationActivities = features
  .filter(f => f.locations_markers.length > 0)
  .groupBy(f => f.locations_markers[0]);
```

### Integration Benefits

Using feature_catalog.json with LLMs provides:
- **Consistency**: All generated content uses same source data
- **Accuracy**: Code references ensure information matches implementation  
- **Scalability**: New features automatically available for content generation
- **Maintenance**: Single source of truth reduces documentation drift
- **Automation**: Reduces manual content creation and updates

### Best Practices for LLM Integration

1. **Validate Confidence Scores**: Use confidence values to prioritize reliable features
2. **Cross-Reference Code**: Verify generated content against code_refs when possible
3. **Update Regularly**: Regenerate content when feature_catalog.json changes
4. **Test Generated Content**: Verify procedures work on live server
5. **Maintain Human Oversight**: Review AI-generated content for accuracy and tone

## File Maintenance

### feature_catalog.json Updates
- Maintain consistent schema across all entries
- Update confidence scores when features change
- Add new features with complete data structures
- Preserve backward compatibility for automated systems

### Integration Testing
- Validate JSON structure with automated tools
- Test LLM prompts with representative feature subsets
- Verify generated content accuracy against live server
- Monitor generated content quality and relevance

## Contributing to Technical Documentation

When updating technical documentation:

1. **Maintain Schema**: Follow established JSON structure exactly
2. **Verify Code References**: Ensure all file paths and line numbers are current
3. **Update Confidence**: Adjust confidence scores based on testing
4. **Document Changes**: Note significant modifications in commit messages
5. **Test Integration**: Verify LLM compatibility after major updates

For detailed contribution guidelines, see [../../CONTRIBUTING.md](../../CONTRIBUTING.md).