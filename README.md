# Common Framework for BWAPI AI - Design

Don't reinvent the wheel! AI development in BWAPI can be a lot easier with a common framework to build on. This repository collects ideas and design documents for a proposed common Starcraft AI framework.

## Design Philosophy
- Expressive and clean API. Provide for concise and beautiful code.
- High level of abstraction. Should be as easy as possible to start programming without worrying about the small details.
- Allow fine-tuning specifics. One size doesn't fit all, and users may need to tweak behavior by overriding or configuring components.
- Modular components. Don't want to be encumbered by a framework? The lower level libraries can be directly used.
- Provide a platform for wrappers in other languages. The public interface must be easy to wrap.
- Because of these considerations, this framework should be written in C++.

## Requirements
- Cross-platform compiler support (clang, msvc, gcc)
- Ready to use in one package. Easy to get started.
- Well documented.
- Testable.

## Components
- Map analysis (BWEM?)
- Building placer
- Build order generator
- Worker manager
- Squad manager
- Wrapper around BWAPI::Unit

### Ideas
- Can we support TorchCraft as well?
- Better than state machines: asynchronous concurrent programming with coroutines/await/actors.
- Take the best components of the existing open-source projects: BWSAL, Skynet, Iron, UAB.

## Contribute your ideas
- Open an issue on this repository for discussion.
- IRC: #BWAPI on freenode http://webchat.freenode.net/?channels=BWAPI
- Forums: http://forum.starcraftai.com/
- BWAPI Wiki: http://www.starcraftai.com/wiki/Main_Page
