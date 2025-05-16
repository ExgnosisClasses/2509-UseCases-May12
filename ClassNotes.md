I like to do an Operation Verification [Content Diagram (OV-1)] Concept, System Functional [Block Definition Diagram (bdd)] and System Decomposition (bdd) before developing a Use Case Diagram. Is this common practice?

### Use Case
- Story or narrative.
- Generic - abstract reference "customer" "account"
- There are multiple alternatives

### Scenario
- A specific execution of the use case with that follows one of the possible paths
- Often referred to as "extensions"
- We cannot document or test ALL of the scenarios - too many

### MoA sky helicopter with a 2 ton capacity is transporting a 1 ton shelter use case
- Document all the alternatives for the use case without listing
- Logic diagram
- Select concrete data vales to test alternatives

---

## Class project

- new use cases for shelter 
- User interface - adding capabilities - testing use cases
- Requirements of the shelter
- requirements -> test process.

Assume we already this shelter.
- requirements that may exist but are not currently implemented
- requirements analysis
- what do the new use cases look like
- Develop user interface - use case
- Generate a test strategy and test plan

Putative Requirements
- Helicopter transport capability
- Internet connectivity
- Environmental system control (Toxic environments)
- Power capabilities
- Weight and dimensions

Scoping

1. the problem to be solved
2. potential solution
3. what is not included in the solution

Helicopter Transport Capability

The problem:

- relocating a shelter to a inaccessible region without an airstrip (no flying with planes)
- What would that look like:
  - how do lift it? Are there current capabilities that we can leverage?
  - Is that going to solve the problem?
  - Sky crane? Are they available to be a solution.
  - Skill sets? needs pilot skills.
  
General Requirements
- Safety - the solution meets all mandated safety requirements
- Manpower availability is suffient to make solution work.

Assumptions
- Personel transportation (in scope or out) -> out of scope
- Assuming we can solve loading issues eg centre of gravity


Scope:
- Personel transport out of scope - moving the shelter
- retrofitting shelters or creating transportable shelter


Stakeholders:
- Pilot and air crew: operational requirements
- Arrival and departure site crew. ATC and ground crew 
- Engineers
  - Helicopter mechanical engineer
  - Maintenance engineers 
  - Supply - cables etc 
  - Conversion engineers - implementing physical solution 
  - Survey and environment
- Logistics 
- End users
  - Diaster response teams
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

#### Main success scenario - Move shelter

- Shelter prepared for transit (create a sub use case to describe the prep process)
- Flies to landing zone
- Shelter deposited and setup

### Main success scenario for Prep shelter

#### Precondition
- Shelter is portioned where it can be accessed by helicopter
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
- alert on checklist
- weather issue
- missing personnel 

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

---

## Determine engineering required for making a shelter transportable by helicopter

###  Can we modify the engineering of an existing shelter design to become transportable by heli

### Putative solutions: 

- Modifications to existing shelter to adapt to new air transport requirement

### Stakeholders

- Pilots requirements relating to flight performance
- Cargo crew chief standards - safety 
- Owner of shelter - durability and integrity of the shelter in transit
  - Do different owners have require
- FAA regs / ATC
- Manufacturer
  - Can the appropriate mods be done?
  - DO we need a redesign
- Ground crew - operation issues 
  - Training requirements
- Hook up and landing times 

### Requirements
- (pilot) Flight characteristics must not be affected too much
- (ground crew) Easy attachment system that can be visually confirm
S
### Solution description
- High level description of the solution and its architecture and moving
- Create simulations for practicality
- alternatives might suggest themselves
- DDifferent ways of making a shelter liftable
- Can we adapt existing and proven solution


### Feasibilty Analysis
- Can we even move a shelter this way structually
  - Unit test, lift a shelter to see if it maintains integrity
- Is there airlift capabilites
  - If no, end of project
- If we need to retrofit - cost and time
- Is there sufficent need?
- Risk profile? 
- Can we provide operational support?

### Protyping - proof of concept
- Start to write the uses for use of each proposed solution
- Create a physical prototype
- Unit test the prototype
- Integration testing shelter protype + helicopter 
- Looking are running through the use cases
  - Hooking up a shelter
  - Moving the shelter
  - Landing the shelter
- Looking for possible points of failure

### Design phase
- Physical designs
- Procedures or the use case descriptions as to how to do this
- Actors
  - Pilot use cases
    - Happy path use case
    - Alternative paths
      - Thing that can go wrong
      - DDifferent kinds of situations
      - Stealth operations
      - Evasive scenario
    - From the pilots - collaboration with the stakeholder
  - Ground crew
    - Issues that they have to deal with and their remediations for things can go wrong
  - Owner of the shelter
    - sSecuring a shelter
    - Testing that it is secure
    - Activating after landing

## Construction
- Shelter construction 

## Deployment and Support
- New use cases
- Actor - logistics and engineering
  - maintenance use cases
  - enhancements
  - new types of tech

## Retirement
- retirement plane 

---

### Current state

1. There are three primary objects - helicopter, shelter, lift harness
2. Agents: pilot, crew chief, ground crew worker, owner representative

- harness can only be attached if the heli is landed
- should be attached to the shelter first
- the harness must be approved by the crew chief after attachment and before use
- The owner rep must certify that the shelter is locked down correctly for transport
- Appriate clearances have been received from ATC and related oversight
- We have acceptance sign off on whether the landing site is usable
- Preflight check verification  
- Loading requirements (weights and dimensions)
- Confirmed structural compliance

Use case for takeoff

GOAL: have the shelter tranport start successful - shelter in now en route.

- Confirm prerequisites by inventorying all required staff and equipment
  - We have all equipment and staff required
- Position helicopter and confirm GO status
  - this may be a precondition
  - All check passed
- Confirm landing zone and ATC clearance 
  - Breaking down landing zone check into detailed steps
  - Break down ATC into specifics - weather, etc
- Inspect shelter for transport compliance
- Inspect harness for defects
- Attach harness to helio
- Test attachment to ensure it was done correctly
- attach harness to shelter
- test attachment
- Start helio up
- Lift test - lift the attachment and wait until confirmation.. load balance, sway
- start transport


---

## Roles

- Roles are arbitrary - they don't map directly to specific jobs or people
- Assign people to roles - or other systems or anything can take action.
- Define the roles
- Assign responsibility to the roles

- Ground crew member 
  - Certified ground crew capable
  - there may be many
- Ground crew chief
  - Is also ground crew member
  - is only one
  - should have lead ground crew training
- Air crew
  - air crew certified
  - there may be many
- Pilot
  - Air crew
  - certified pilot
  - only one
- Product owner
  - represent the owner of the shelter
  - Authorized by the owner
- ATC
  - Any flight oversight authority
  - If multiple, no over responsibility


