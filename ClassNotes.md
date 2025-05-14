I like to do an Operation Verification [Content Diagram (OV-1)] Concept, System Functional [Block Definition Diagram (bdd)] and System Decomposition (bdd) before developing a Use Case Diagram. Is this common practice?

### Use Case
- Story or narrative.
- Generic - abstract reference "customer" "account"
- There are multiple alternatives

### Scenario
- A specific execution of the use case with that follows one of the possible paths
- Often referred to as "extensions"
- We cannot document or test ALL of the scenarios - too many

### MOdern use case
- Document all the alternatives for the use case without listing
- Logic diagram
- Select concrete data vales to test alternatives

---

## Class project

- new use cases for shelter 
- User interace - adding capabilites - testing use cases
- Requirements of the shelter
- requirements -> test process.

Assume we already this shelter.
- requirements that may exist but are not currently implented
- requirements analysis
- what do the new use cases look like
- Develop user interface - use case
- Generate a test strategy and test plan

Putative Requirements
- Helicopter transport capability
- Internet connectivity
- Environmental system control (Toxic environments)
- Power capbilities
- Weight and dimensions

Scoping

1. the problem to be solved
2. potential solution
3. what is not included in the solution

Helicopter Transport Capabilty

The problem:

- relocating a shelter to a inaccessible region without an airstrip (no flying with places)
- What would that look like:
  - how do lift it? Are there current capabilites that we can leverage?
  - Is that going to solve the problem?
  - Sky crane? Are they available to be a solution.
  - Skill sets? needs pilot skills>
  
General Requirements
- Safety - the solution meets all mandated safety requirements
- Manpower availability is suffient to make solution work.

Assumptions
- Personel transportion (in scope or out)
- Assuming we can solve loading issues eg centre of gravity


Scope:
- Personel transport out of scope - moving the shelter


Stakeholders:
- Pilot and air crew: operational requirements
- Arrival and departuew site crew. ATC and ground crew 
- Engineers
  - Helicopter mechanical engineer
  - Maintence engineers 
  - Supply - cables etc 
  - Conversion engineers - implementing physical solution 
  - Survey and environment
- Logistics 
- End users
  - Diaster reponse teams
    - Speed of deployment
    - Environment condition reliance 
  - Police operation
    - Stealth Capability

## Goal Levels
1. Strategic: Move the shelter
2. Tactical: Hooking up, moving, landing, unhooking and setting up
3. Operational: Steps required to accomplish a tactical goal

## Use Cases:

### Deployment

#### Preconditions
- Helicopter with appropriate mods is available
- Pilot and crew trained in hooking it up
- Shelter has the apprpriate mods

#### Main success senario - Move shelter

- Shelter preped for transit (create a sub use case to describe the prep process)
- Flies to landing zone
- Shelter deposited and setup

### Main success scenario for Prep shelter

#### Precondition
- Shelter is postioned where it can be accessed by helicopter
- Helicopter is rigged to transport

1. Secure shelter for transport - power down, secure contents and verify
2. Crew briefing, pre flight checklist and operational review
3. Attach and secure and check cables - lift harness - to shelter
4. Attache lift harness the helicopter
5. Safety check and review
6. Lift off - get airborn

Step 1:
- cannot finish prep

Step 2:
- altert on checklist
- weather issue
- missing personel 

---

## Testing 

- Unit testing: Testing individual components (functional)
- Integration testing: Testing all components together (functional)
- Performance testing: Non functional requirements
- end to end testing (e2e) - running selected scenarios as test cases
- Acceptance testing


Unit helicopter lift assembly
Unit test shelter
Integration test  = shelter + helicopter

Main success
A sky helicopter with a 2 ton capacity is transporting a 1 tone shelter

Overweight scenario (examples)
A sky helicopter with a 2 ton capacity is transporting a 3 ton shelter
Outcome: failed safety check

Given helio lift capacity is 2 tons
- shelter is 1.9  tons
- shelter is 2.1 tons