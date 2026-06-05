# Filmography

Filmography is a complete film and video production methodology for your coding agents, adapted from the Superpowers framework. It provides a set of composable skills and initial instructions that help agents coordinate all aspects of production—from screenwriting and directing to cinematography, lighting, and post-production.

## What is Filmography?

Filmography is an agentic skills framework designed for creative collaboration in film production. Instead of jumping straight into shooting, it steps back and asks the right questions first:

1. **Brainstorming** - Refine the creative vision through dialogue
2. **Story Development** - Build screenplay and narrative structure
3. **Production Planning** - Create shot lists, schedules, and budgets
4. **Directing** - Coordinate actors, camera movement, and scene flow
5. **Cinematography** - Plan camera angles, lighting, composition
6. **Gaffer Work** - Technical lighting specifications
7. **Production Coordination** - Manage crew, locations, equipment
8. **Post-Production** - Editing, color grading, sound design

## How it Works

The framework provides **Skills** (best practice guides for each production role) and **Agents** (specialized agents for Screenwriter, Director, Cinematographer, Gaffer, Producer, and Post-Production Lead).

Agents use these skills to:
- Ask clarifying questions about creative vision
- Propose multiple approaches with trade-offs
- Create detailed production plans
- Coordinate between departments
- Verify quality and consistency
- Make data-driven decisions

## Core Skills

### Creative Development
- **brainstorming** - Refine creative concepts through collaborative dialogue
- **screenwriting** - Story structure, character development, dialogue
- **story-development** - Narrative arc, pacing, emotional beats

### Production Departments
- **directing** - Shot planning, actor direction, scene coordination
- **cinematography** - Camera movement, composition, visual language
- **gaffer-work** - Lighting design and technical specifications
- **production-planning** - Scheduling, budgeting, logistics
- **locations-scouting** - Location assessment and documentation

### Execution & Review
- **production-coordination** - Department coordination and scheduling
- **requesting-production-review** - Quality checks across departments
- **post-production** - Editing, color grading, sound design
- **systematic-problem-solving** - Troubleshooting production issues

### Meta
- **writing-skills** - Create new production skills
- **using-filmography** - Introduction to the framework

## Installation

### Claude Code

```bash
/plugin install filmography@umer2001/filmography
```

### Cursor

```bash
/add-plugin filmography
```

### Other Harnesses

Register the marketplace and install:

```bash
plugin marketplace add umer2001/filmography
plugin install filmography@filmography-marketplace
```

## Basic Workflow

1. **Brainstorming** - Explore creative vision, constraints, and success criteria
2. **Story Development** - Write screenplay, develop characters, establish narrative
3. **Production Planning** - Create shot lists, shot schedules, production timeline
4. **Department Planning** - Each department (Camera, Lighting, Sound, Wardrobe) creates specifications
5. **Production Coordination** - Dispatch agents for each department, coordinate schedules
6. **On-Set Execution** - Directors, cinematographers, gaffers execute their plans
7. **Production Review** - Verify work quality, consistency, and plan adherence
8. **Post-Production** - Editing, color correction, sound design, final delivery

## Philosophy

- **Systematic over ad-hoc** - Process over guessing
- **Collaboration over siloing** - Clear communication between departments
- **Specification before execution** - Planning before production
- **Evidence over claims** - Review and verify before approving
- **Incremental validation** - Get approval after each phase

## The Production Agents

### Screenwriter
Focuses on story structure, character development, dialogue, and narrative pacing. Ensures the script is complete, coherent, and ready for production.

### Director
Coordinates the overall creative vision. Plans shots, directs actors, manages scene flow, and ensures narrative consistency. Acts as the central creative authority.

### Cinematographer
Plans camera movement, composition, visual language, and technical camera specifications. Works with the Director to realize the visual vision.

### Gaffer (Chief Lighting Technician)
Designs lighting setups, specifies equipment, and creates technical lighting documentation. Ensures lighting supports the visual language and mood.

### Producer
Manages scheduling, budgeting, logistics, and resources. Coordinates between departments and solves production problems.

### Post-Production Lead
Oversees editing, color grading, sound design, and final delivery. Ensures post-production work aligns with the original creative vision.

## Contributing

Contributions are welcome! Please follow these guidelines:

1. Fork the repository
2. Create a branch for your work
3. Follow the `writing-skills` skill for creating production skills
4. Submit a pull request with a clear description

See `CLAUDE.md` for detailed contributor guidelines.

## License

MIT License - see LICENSE file for details

## Community

Filmography is built for creative professionals using AI agents to coordinate complex productions.

- **GitHub Issues**: https://github.com/umer2001/filmography/issues
- **Discussions**: https://github.com/umer2001/filmography/discussions
- **Documentation**: https://github.com/umer2001/filmography
