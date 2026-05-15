# Compliance Training Storyboard Skill

A compliance training storyboard generator grounded in strong instructional design principles, adaptable to any organisation or regulatory context.

## Overview

This skill transforms raw compliance content into a complete, instructionally sound storyboard for eLearning development. It is designed for use by compliance subject matter experts (SMEs) who are knowledgeable in regulations but not trained in instructional design.

## Features

- **User-Centric Design**: Content is clear, intuitive, and easy to navigate
- **Engaging Storytelling**: Training reads as a cohesive, purposeful narrative
- **On-Brand Relevance**: Examples and scenarios aligned to organizational context
- **Evolving with Agility**: Modular structure that's easy to update

## Target Users

**Primary users:** Compliance subject matter experts (SMEs) who are knowledgeable in regulations but not trained in instructional design.

**Input:** Draft compliance content — structured documents, slide decks, policy documents, regulatory outlines, or draft training material.

**Output:** A complete `.docx` storyboard ready for review and handoff to learning designers.

## Key Capabilities

### Learning Design
- Generates 3-5 learning objectives using Bloom's Taxonomy (levels 1-4)
- Creates logical, learner-friendly course structure (30-60 minutes)
- Includes strategic scenarios (max 3 per course)
- Provides cumulative knowledge assessments

### Content Standards
- Maintains regulatory accuracy without reinterpretation
- Applies consistent document formatting (Montserrat font, black text)
- Includes specific, actionable visual suggestions
- Supports localization (UK/Australian English conventions)

### Instructional Features
- Video narration scripts for introductions
- Interactive scenarios with decision points
- Knowledge check questions with feedback
- Resource links and next steps

## Compliance Constraints

- **Regulatory Accuracy**: Never alters the meaning or intent of original regulatory content
- **Course Length**: Maximum 1 hour duration
- **Scenario Limit**: Maximum 3 scenarios per course, grounded in source material
- **Content Scope**: Only covers concepts present in source material

## File Structure

```
compliance-storyboard-skill/
├── SKILL.md                 # Main skill instructions and templates
├── references/
│   └── hr-workplace.md      # HR & workplace compliance reference
└── README.md               # This file
```

## Usage Triggers

Use this skill when users mention:
- "storyboard"
- "compliance training" 
- "eLearning module"
- "course outline"
- "training script"
- Converting policy/regulation documents into training courses
- Writing learning objectives, narration scripts, knowledge checks, or interactive scenarios

## Dependencies

- Requires `docx` skill for generating Word document output
- Integrates with instructional design frameworks (Bloom's Taxonomy, Gagné's Nine Events, etc.)

## Quality Standards

Every storyboard output includes:
- ✅ Learning objectives in Course Overview (not as lesson screens)
- ✅ Narration only for Video and Scenario screens
- ✅ Specific, actionable visual suggestions for every screen
- ✅ Cumulative assessment covering all objectives
- ✅ Consistent formatting and localization
- ✅ Regulatory language accuracy maintained

## Version

Current version: 1.0
Last updated: May 2026

## License

This skill is part of the goose agent framework and follows the same licensing terms.