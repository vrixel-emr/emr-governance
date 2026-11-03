# Healthcare EMR: architecture overview

The current design, kept by the product's architects. Agents read this before every design; it
changes through pull requests like any governance file. Decisions are in `decisions/`.

## Context

AI-native electronic medical records for US and India clinics. Users: clinicians, front-desk
staff and patients. Every system boundary speaks FHIR R4. Regulation: HIPAA in the US, ABDM in
India. All patient data is PHI.

## Building blocks

None yet. The first feature's design proposes the EMR's repositories, each with an ADR; G4
approves them and the SDLC creates them from the platform templates. This section then lists each
repository, its role and what it owns.

Shared services (`SS` lane) provide platform packages, including `ss-llm-gateway`, which the EMR
deploys in its own OpenChoreo project `emr`. Payments go through APX (`APX` lane).

## Change log
