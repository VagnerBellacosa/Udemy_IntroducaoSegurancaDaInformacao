# Fail-safe

From Wikipedia, the free encyclopedia

[Jump to navigation](https://en.wikipedia.org/wiki/Fail-safe#mw-head)[Jump to search](https://en.wikipedia.org/wiki/Fail-safe#searchInput)

For other uses, see [Fail-safe (disambiguation)](https://en.wikipedia.org/wiki/Fail-safe_(disambiguation)).

In [engineering](https://en.wikipedia.org/wiki/Engineering), a **fail-safe** is a design feature or practice that in the event of a specific type of [failure](https://en.wikipedia.org/wiki/Failure_causes), inherently responds in a way that will cause minimal or no harm to other equipment, to the environment or to people. Unlike [inherent safety](https://en.wikipedia.org/wiki/Inherent_safety) to a particular hazard, a system being "fail-safe" does not mean that failure is impossible or improbable, but rather that the system's design prevents or mitigates unsafe consequences of the system's failure. That is, if and when a "fail-safe" system fails, it remains at least as safe as it was before the failure.[[1\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-1)[[2\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-2) Since many types of failure are possible, [failure mode and effects analysis](https://en.wikipedia.org/wiki/Failure_mode_and_effects_analysis) is used to examine failure situations and recommend safety design and procedures.

Some systems can never be made fail-safe, as continuous availability is needed. [Redundancy](https://en.wikipedia.org/wiki/Redundancy_(engineering)), [fault tolerance](https://en.wikipedia.org/wiki/Fault_tolerance), or [contingency plans](https://en.wikipedia.org/wiki/Contingency_plan) are used for these situations (e.g. multiple independently controlled and fuel-fed engines).[[3\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-3)

## Contents



- 1Examples
  - [1.1Mechanical or physical](https://en.wikipedia.org/wiki/Fail-safe#Mechanical_or_physical)
  - [1.2Electrical or electronic](https://en.wikipedia.org/wiki/Fail-safe#Electrical_or_electronic)
  - [1.3Procedural safety](https://en.wikipedia.org/wiki/Fail-safe#Procedural_safety)
- 2Other terminology
  - [2.1Fail safe and fail secure](https://en.wikipedia.org/wiki/Fail-safe#Fail_safe_and_fail_secure)
  - [2.2Fail active operational](https://en.wikipedia.org/wiki/Fail-safe#Fail_active_operational)
  - [2.3Failsafe point](https://en.wikipedia.org/wiki/Fail-safe#Failsafe_point)
- [3See also](https://en.wikipedia.org/wiki/Fail-safe#See_also)
- [4References](https://en.wikipedia.org/wiki/Fail-safe#References)

## Examples[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=1)]

### Mechanical or physical[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=2)]

[![img](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Pl_control_valve.jpg/220px-Pl_control_valve.jpg)](https://en.wikipedia.org/wiki/File:Pl_control_valve.jpg)

Globe control valve with pneumatic diaphragm actuator. Such a valve can be designed to fail to safety using spring pressure if the actuating air is lost.

Examples include:

- Roller-shutter fire doors that are activated by building alarm systems or local smoke detectors must close automatically when signaled regardless of power. In case of power outage the coiling fire door does not need to close, but must be capable of automatic closing when given a signal from the building alarm systems or smoke detectors. A temperature-sensitive [fusible link](https://en.wikipedia.org/wiki/Fusible_link) may be employed to hold the fire doors open against gravity or a closing spring. In case of fire, the link melts and releases the doors, and they close.
- Some airport [baggage](https://en.wikipedia.org/wiki/Baggage) [carts](https://en.wikipedia.org/wiki/Cart) require that the person hold down a given cart's handbrake switch at all times; if the handbrake switch is released, the brake will activate, and assuming that all other portions of the braking system are working properly, the cart will stop. The handbrake-holding requirement thus both operates according to the principles of "fail-safety" and contributes to (but does not necessarily ensure) the fail-security of the system. This is an example of a *[dead man's switch](https://en.wikipedia.org/wiki/Dead_man's_switch)*.
- [Lawnmowers](https://en.wikipedia.org/wiki/Lawnmower) and [snow blowers](https://en.wikipedia.org/wiki/Snow_blower) have a hand-closed lever that must be held down at all times. If it is released, it stops the blade's or rotor's rotation. This also functions as a *dead man's switch*.
- [Air brakes](https://en.wikipedia.org/wiki/Air_brake_(rail)) on railway [trains](https://en.wikipedia.org/wiki/Train) and [air brakes](https://en.wikipedia.org/wiki/Air_brake_(road_vehicle)) on [trucks](https://en.wikipedia.org/wiki/Truck). The brakes are held in the "off" position by air [pressure](https://en.wikipedia.org/wiki/Pressure) created in the brake system. Should a brake line split, or a carriage become de-coupled, the air pressure will be lost and the brakes applied, by springs in the case of trucks, or by a local air reservoir in trains. It is impossible to drive a truck with a serious leak in the air brake system. (Trucks may also employ [wig wags](https://en.wikipedia.org/wiki/Wig_wag_(truck_braking_systems)) to indicate low air pressure.)
- Motorized gates – In case of power outage the gate can be pushed open by hand with no crank or key required. However, as this would allow virtually anyone to go through the gate, a *fail-secure* design is used: In a power outage, the gate can only be opened by a hand crank that is usually kept in a safe area or under lock and key. When such a gate provides vehicle access to homes, a fail-safe design is used, where the door opens to allow fire department access.
- Safety valves – Various devices that operate with [fluids](https://en.wikipedia.org/wiki/Fluid) use [fuses](https://en.wikipedia.org/wiki/Fuse_(hydraulic)) or [safety valves](https://en.wikipedia.org/wiki/Safety_valve) as fail-safe mechanisms.

[![img](https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/130330_Thomas_ELC_and_Wansbeck_Railtour_Northumberlandia_030.jpg/220px-130330_Thomas_ELC_and_Wansbeck_Railtour_Northumberlandia_030.jpg)](https://en.wikipedia.org/wiki/File:130330_Thomas_ELC_and_Wansbeck_Railtour_Northumberlandia_030.jpg)

Railway semaphore signals. "Stop" or "caution" is a horizontal arm, "Clear to Proceed" is 45 degrees upwards, so failure of the actuating cable releases the signal arm to safety under gravity.

- A [railway semaphore signal](https://en.wikipedia.org/wiki/Railway_semaphore_signal) is specially designed so that, should the cable controlling the signal break, the arm returns to the "danger" position, preventing any trains passing the inoperative signal.
- [Isolation valves](https://en.wikipedia.org/wiki/Isolation_valve), and control valves, that are used for example in systems containing hazardous substances, can be designed to close upon loss of power, for example by spring force. This is known as fail-closed upon loss of power.
- An [elevator](https://en.wikipedia.org/wiki/Elevator) has brakes that are held off brake pads by the tension of the elevator cable. If the cable breaks, tension is lost and the brakes latch on the rails in the shaft, so that the elevator cabin does not fall.
- Vehicle air conditioning – Defrost controls require vacuum for diverter damper operation for all functions except defrost. If vacuum fails, defrost is still available.

### Electrical or electronic[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=3)]

Examples include:

- Many devices are protected from [short circuit](https://en.wikipedia.org/wiki/Short_circuit) by [fuses](https://en.wikipedia.org/wiki/Fuse_(electrical)), [circuit breakers](https://en.wikipedia.org/wiki/Circuit_breaker), or [current limiting](https://en.wikipedia.org/wiki/Current_limiting) circuits. The electrical interruption under overload conditions will prevent damage or destruction of wiring or circuit devices due to overheating.
- [Avionics](https://en.wikipedia.org/wiki/Avionics) using [redundant systems](https://en.wikipedia.org/wiki/Redundancy_(engineering)) to perform the [same computation using three different systems](https://en.wikipedia.org/wiki/Triple_modular_redundancy). Different results indicate a fault in the system.[[4\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-4)
- [Drive-by-wire](https://en.wikipedia.org/wiki/Drive-by-wire) and [fly-by-wire](https://en.wikipedia.org/wiki/Fly-by-wire) controls such as an Accelerator Position Sensor typically have two potentiometers which read in opposite directions, such that moving the control will result in one reading becoming higher, and the other generally equally lower. Mismatches between the two readings indicates a fault in the system, and the [ECU](https://en.wikipedia.org/wiki/Engine_control_unit) can often deduce which of the two readings is faulty.[[5\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-5)
- [Traffic light](https://en.wikipedia.org/wiki/Traffic_light) controllers use a *Conflict Monitor Unit* to detect faults or conflicting signals and switch an intersection to an all flashing error signal, rather than displaying potentially dangerous conflicting signals, e.g. showing [green](https://en.wikipedia.org/wiki/Green) in all directions.[[6\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-6)
- The automatic protection of programs and/or processing systems when a [computer hardware](https://en.wikipedia.org/wiki/Computer_hardware) or [software](https://en.wikipedia.org/wiki/Software) failure is detected in a [computer system](https://en.wikipedia.org/wiki/Computer_system). A classic example is a [watchdog timer](https://en.wikipedia.org/wiki/Watchdog_timer). See [Fail-safe (computer)](https://en.wikipedia.org/wiki/Fail-safe_(computer)).
- A [control operation](https://en.wikipedia.org/wiki/Control_operation) or function that prevents improper system functioning or [catastrophic](https://en.wikipedia.org/wiki/Catastrophic_failure) degradation in the event of [circuit](https://en.wikipedia.org/wiki/Electronic_circuit) malfunction or operator error; for example, the failsafe [track circuit](https://en.wikipedia.org/wiki/Track_circuit) used to control [railway block signals](https://en.wikipedia.org/wiki/Railway_signalling). The fact that a flashing amber is more permissive than a solid amber on many railway lines is a sign of a failsafe, as the relay, if not working, will revert to a more restrictive setting.
- The iron pellet ballast on the [Bathyscaphe](https://en.wikipedia.org/wiki/Bathyscaphe) is dropped to allow the submarine to ascend. The ballast is held in place by [electromagnets](https://en.wikipedia.org/wiki/Electromagnet). If electrical power fails, the ballast is released, and the submarine then ascends to safety.
- Many [nuclear reactor](https://en.wikipedia.org/wiki/Nuclear_reactor) designs have neutron absorbing control rods suspended by electromagnets. If the power fails, they drop under gravity into the core and shut down the chain reaction in seconds by absorbing the neutrons needed for fission to continue.
- In [industrial automation](https://en.wikipedia.org/wiki/Industrial_automation), alarm circuits are usually "[normally closed](https://en.wikipedia.org/wiki/Normally_closed)". This ensures that in case of a wire break the alarm will be triggered. If the circuit were normally open, a wire failure would go undetected, while blocking actual alarm signals.
- Analog sensors and modulating actuators can usually be installed and wired such that the circuit failure results in an out-of-bound reading – see [current loop](https://en.wikipedia.org/wiki/Current_loop). For example, a potentiometer indicating pedal position might only travel from 20% to 80% of its full range, such that a cable break or short results in a 0% or 100% reading.
- In control systems, critically important signals can be carried by a complementary pair of wires (<signal> and <not_signal>). Only states where the two signals are opposite (one is high, the other low) are valid. If both are high or both are low the control system knows that something is wrong with the sensor or connecting wiring. Simple failure modes (dead sensor, cut or unplugged wires) are thereby detected. An example would be a control system reading both the [normally open](https://en.wikipedia.org/wiki/Normally_open) (NO) and [normally closed](https://en.wikipedia.org/wiki/Normally_closed) (NC) poles of a [SPDT](https://en.wikipedia.org/wiki/Switch#Contact_terminology) selector switch against common, and checking them for coherency before reacting to the input.
- In [HVAC control systems](https://en.wikipedia.org/wiki/HVAC_control_system), [actuators](https://en.wikipedia.org/wiki/Actuators) that control dampers and valves may be fail-safe, for example, to prevent coils from freezing or rooms from overheating. Older [pneumatic actuators](https://en.wikipedia.org/wiki/Pneumatic_actuators) were inherently fail-safe because if the air pressure against the internal diaphragm failed, the built-in spring would push the actuator to its home position – of course the home position needed to be the "safe" position. Newer electrical and electronic actuators need additional components (springs or capacitors) to automatically drive the actuator to home position upon loss of electrical power.[[7\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-7)
- [Programmable logic controllers](https://en.wikipedia.org/wiki/Programmable_logic_controller) (PLCs). To make a PLC fail-safe the system does not require energization to stop the drives associated. For example, usually, an emergency stop is a [normally closed](https://en.wikipedia.org/wiki/Normally_closed) contact. In the event of a power failure this would remove the power directly from the coil and also the PLC input. Hence, a fail-safe system.
- If a [voltage regulator](https://en.wikipedia.org/wiki/Voltage_regulator) fails, it can destroy connected equipment. A [crowbar (circuit)](https://en.wikipedia.org/wiki/Crowbar_(circuit)) prevents damage by short-circuiting the power supply as soon as it detects overvoltage.

### Procedural safety[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=4)]

[![img](https://upload.wikimedia.org/wikipedia/commons/thumb/8/80/FA-18-Afterburners.jpg/220px-FA-18-Afterburners.jpg)](https://en.wikipedia.org/wiki/File:FA-18-Afterburners.jpg)

An aircraft lights its [afterburners](https://en.wikipedia.org/wiki/Afterburner) to maintain full power during an [arrested landing](https://en.wikipedia.org/wiki/Arrested_landing) aboard an [aircraft carrier](https://en.wikipedia.org/wiki/Aircraft_carrier). If the arrested landing fails, the aircraft can safely take off again.

As well as physical devices and systems fail-safe procedures can be created so that if a procedure is not carried out or carried out incorrectly no dangerous action results. For example:

- Spacecraft trajectory - During early [Apollo program](https://en.wikipedia.org/wiki/Apollo_program) missions to the Moon, the spacecraft was put on a [free return trajectory](https://en.wikipedia.org/wiki/Free_return_trajectory) — if the engines had failed at [lunar orbit](https://en.wikipedia.org/wiki/Lunar_orbit) insertion, the craft would have safely coasted back to Earth.
- The pilot of an aircraft landing on an [aircraft carrier](https://en.wikipedia.org/wiki/Aircraft_carrier) increases the throttle to full power at touchdown. If the [arresting wires](https://en.wikipedia.org/wiki/Arresting_wire) fail to capture the aircraft, it is able to take off again; this is an example of *fail-safe practice*.[[8\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-8)
- In [railway signalling](https://en.wikipedia.org/wiki/Railway_signalling) signals which are not in active use for a train are required to be kept in the 'danger' position. The default position of every controlled absolute signal is therefore "danger", and therefore a positive action — setting signals to "clear" — is required before a train may pass. This practice also ensures that, in case of a fault in the signalling system, an incapacitated signalman, or the unexpected entry of a train, that a train will never be shown an erroneous "clear" signal.
- Railroad engineers are instructed that a railway signal showing a confusing, contradictory or unfamiliar aspect (for example a [colour light signal](https://en.wikipedia.org/wiki/Railway_signalling#Colour_light_signals) that has suffered an electrical failure and is showing no light at all) must be treated as showing "danger". In this way, the driver contributes to the fail-safety of the system.

## Other terminology[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=5)]

Fail-safe ([foolproof](https://en.wikipedia.org/wiki/Idiot_proof)) devices are also known as *[poka-yoke](https://en.wikipedia.org/wiki/Poka-yoke)* devices. *Poka-yoke*, a [Japanese](https://en.wikipedia.org/wiki/Japanese_language) term, was coined by [Shigeo Shingo](https://en.wikipedia.org/wiki/Shigeo_Shingo), a quality expert.[[9\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-9)[[10\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-10) "Safe to fail" refers to civil engineering designs such as the [Room for the River project in Netherlands](https://en.wikipedia.org/wiki/Room_for_the_River_(Netherlands)) and the Thames Estuary 2100 Plan[[11\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-TE2100-11)[[12\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-TE21-12) which incorporate flexible adaptation strategies or [climate change adaptation](https://en.wikipedia.org/wiki/Climate_change_adaptation) which provide for, and limit, damage, should severe events such as 500-year floods occur.[[13\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-TDC032013-13)

### Fail safe and fail secure[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=6)]

*Fail-safe* and *fail-secure* are distinct concepts. *Fail-safe* means that a device will not endanger lives or property when it fails. *Fail-secure,* also called *fail-closed,* means that access or data will not fall into the wrong hands in a security failure. Sometimes the approaches suggest opposite solutions. For example, if a building catches fire, fail-safe systems would unlock doors to ensure quick escape and allow firefighters inside, while fail-secure would lock doors to prevent unauthorized access to the building.

The opposite of *fail-closed* is called *fail-open*.

### Fail active operational[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=7)]

Fail active operational can be installed on systems that have a high degree of redundancy so that a single failure of any part of the system can be tolerated (fail active operational) and a second failure can be detected – at which point the system will turn itself off (uncouple, fail passive). One way of accomplishing this is to have three identical systems installed, and a control logic which detects discrepancies. An example for this are many aircraft systems, among them [inertial navigation systems](https://en.wikipedia.org/wiki/Inertial_navigation_system) and [pitot tubes](https://en.wikipedia.org/wiki/Pitot_tube).

### Failsafe point[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=8)]

During the [Cold War](https://en.wikipedia.org/wiki/Cold_War), "failsafe point" was the term used for the point of no return for American [Strategic Air Command](https://en.wikipedia.org/wiki/Strategic_Air_Command) nuclear bombers, just outside Soviet airspace. In the event of receiving an attack order, the bombers were required to linger at the failsafe point and wait for a second confirming order; until one was received, they would not arm their bombs or proceed further.[[14\]](https://en.wikipedia.org/wiki/Fail-safe#cite_note-14) The design was prevent any single failure of the American command system causing nuclear war. This sense of the term entered the American popular lexicon with the publishing of the 1962 novel *[Fail-Safe](https://en.wikipedia.org/wiki/Fail-Safe_(novel))*.

(Other nuclear war command control systems have used the opposite scheme, [fail-deadly](https://en.wikipedia.org/wiki/Fail-deadly), which requires continuous or regular proof that an enemy first-strike attack has *not* occurred to *prevent* the launching of a nuclear strike.)

## See also[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=9)]

| ![img](https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Wiktionary-logo-en-v2.svg/40px-Wiktionary-logo-en-v2.svg.png) | Look up ***[fail-safe](https://en.wiktionary.org/wiki/fail-safe)*** in Wiktionary, the free dictionary. |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

- [Fail-fast](https://en.wikipedia.org/wiki/Fail-fast)
- [Control theory](https://en.wikipedia.org/wiki/Control_theory)
- [Dead man's switch](https://en.wikipedia.org/wiki/Dead_man's_switch)
- [EIA-485](https://en.wikipedia.org/wiki/EIA-485)
- [Elegant degradation](https://en.wikipedia.org/wiki/Elegant_degradation)
- [Failing badly](https://en.wikipedia.org/wiki/Failing_badly)
- [Fail-deadly](https://en.wikipedia.org/wiki/Fail-deadly)
- [Fault tolerance](https://en.wikipedia.org/wiki/Fault_tolerance)
- [IEC 61508](https://en.wikipedia.org/wiki/IEC_61508)
- [Interlock](https://en.wikipedia.org/wiki/Interlock)
- [Safe-life design](https://en.wikipedia.org/wiki/Safe-life_design)
- [Safety engineering](https://en.wikipedia.org/wiki/Safety_engineering)

## References[[edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit&section=10)]

1. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-1)** "[Fail-safe](http://www.audioenglish.net/dictionary/fail-safe.htm)". AudioEnglich.net. Accessed 2009.12.31
2. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-2)** *e.g.*, David B. Rutherford Jr., [What Do You Mean It\'s Fail Safe?](https://web.archive.org/web/20111008021648/http://www.billpetit.com/Papers/Petit017.pdf) . 1990 Rapid Transit Conference
3. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-3)** Bornschlegl, Susanne (2012). [*Ready for SIL 4: Modular Computers for Safety-Critical Mobile Applications*](https://www.menmicro.com/downloads/search/dl/sk/"White Paper%3A Ready for SIL4%3A Modular Computers for Safety-Critical Mobile Applications"/dx/1/) (pdf). MEN Mikro Elektronik. Retrieved 2015-09-21.
4. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-4)** Bornschlegl, Susanne (2012). [*Ready for SIL 4: Modular Computers for Safety-Critical Mobile Applications*](https://www.menmicro.com/downloads/search/dl/sk/"White Paper%3A Ready for SIL4%3A Modular Computers for Safety-Critical Mobile Applications"/dx/1/) (pdf). MEN Mikro Elektronik. Retrieved 2015-09-21.
5. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-5)** ["P2138 DTC Throttle/Pedal Pos Sensor/Switch D / E Voltage Correlation"](http://www.obd-codes.com/p2138). *www.obd-codes.com*.
6. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-6)** Manual on Uniform Traffic Control Devices, Federal Highway Administration, 2003
7. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-7)** ["When Failure Is Not an Option: The Evolution of Fail-Safe Actuators"](https://www.kmccontrols.com/blog/when-failure-is-not-an-option-the-evolution-of-fail-safe-actuators/). KMC Controls. Retrieved 12 April 2021.
8. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-8)** Harris, Tom. ["How Aircraft Carriers Work"](http://science.howstuffworks.com/aircraft-carrier4.htm). *HowStuffWorks, Inc*. Retrieved 2007-10-20.
9. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-9)** Shingo, Shigeo; Andrew P. Dillon (1989). A study of the Toyota production system from an industrial engineering viewpoint. Portland, Oregon: Productivity Press. p. 22. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier)) [0-915299-17-8](https://en.wikipedia.org/wiki/Special:BookSources/0-915299-17-8). [OCLC](https://en.wikipedia.org/wiki/OCLC_(identifier)) [19740349](https://www.worldcat.org/oclc/19740349)
10. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-10)** John R. Grout, Brian T. Downs. "A Brief Tutorial on Mistake-proofing, Poka-Yoke, and ZQC", [MistakeProofing.com](http://www.mistakeproofing.com/tutorial.html)
11. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-TE2100_11-0)** ["Thames Estuary 2100 Plan"](http://webarchive.nationalarchives.gov.uk/20121210131034/http://www.environment-agency.gov.uk/static/documents/Leisure/SE_TE2100_briefing.pdf) (PDF). UK Environment Agency. November 2012. Archived from [the original](http://www.environment-agency.gov.uk/static/documents/Leisure/SE_TE2100_briefing.pdf) (PDF) on 2012-12-10. Retrieved March 20, 2013.
12. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-TE21_12-0)** ["Thames Estuary 2100 (TE2100)"](http://www.environment-agency.gov.uk/homeandleisure/floods/125045.aspx). UK Environment Agency. Retrieved March 20, 2013.
13. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-TDC032013_13-0)** Jennifer Weeks (March 20, 2013). ["Adaptation expert Paul Kirshen proposes a new paradigm for civil engineers: 'safe to fail,' not 'fail safe'"](https://web.archive.org/web/20130513080832/http://wwwp.dailyclimate.org/tdc-newsroom/2013/03/flexible-infrastructure-climate-stress). *The Daily Climate*. Archived from [the original](http://wwwp.dailyclimate.org/tdc-newsroom/2013/03/flexible-infrastructure-climate-stress) on May 13, 2013. Retrieved March 20, 2013.
14. **[^](https://en.wikipedia.org/wiki/Fail-safe#cite_ref-14)** ["fail-safe"](https://www.dictionary.com/browse/failsafe). *Dictionary.com*. Retrieved November 7, 2021.

[Categories](https://en.wikipedia.org/wiki/Help:Category): 

- [Safety](https://en.wikipedia.org/wiki/Category:Safety)
- [Fault tolerance](https://en.wikipedia.org/wiki/Category:Fault_tolerance)
- [Fault-tolerant computer systems](https://en.wikipedia.org/wiki/Category:Fault-tolerant_computer_systems)

## Navigation menu

- Not logged in
- [Talk](https://en.wikipedia.org/wiki/Special:MyTalk)
- [Contributions](https://en.wikipedia.org/wiki/Special:MyContributions)
- [Create account](https://en.wikipedia.org/w/index.php?title=Special:CreateAccount&returnto=Fail-safe)
- [Log in](https://en.wikipedia.org/w/index.php?title=Special:UserLogin&returnto=Fail-safe)

- [Article](https://en.wikipedia.org/wiki/Fail-safe)
- [Talk](https://en.wikipedia.org/wiki/Talk:Fail-safe)

- [Read](https://en.wikipedia.org/wiki/Fail-safe)
- [Edit](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=edit)
- [View history](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=history)

### Search

- [Main page](https://en.wikipedia.org/wiki/Main_Page)
- [Contents](https://en.wikipedia.org/wiki/Wikipedia:Contents)
- [Current events](https://en.wikipedia.org/wiki/Portal:Current_events)
- [Random article](https://en.wikipedia.org/wiki/Special:Random)
- [About Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:About)
- [Contact us](https://en.wikipedia.org/wiki/Wikipedia:Contact_us)
- [Donate](https://donate.wikimedia.org/wiki/Special:FundraiserRedirector?utm_source=donate&utm_medium=sidebar&utm_campaign=C13_en.wikipedia.org&uselang=en)

### Contribute

- [Help](https://en.wikipedia.org/wiki/Help:Contents)
- [Learn to edit](https://en.wikipedia.org/wiki/Help:Introduction)
- [Community portal](https://en.wikipedia.org/wiki/Wikipedia:Community_portal)
- [Recent changes](https://en.wikipedia.org/wiki/Special:RecentChanges)
- [Upload file](https://en.wikipedia.org/wiki/Wikipedia:File_Upload_Wizard)

### Tools

- [What links here](https://en.wikipedia.org/wiki/Special:WhatLinksHere/Fail-safe)
- [Related changes](https://en.wikipedia.org/wiki/Special:RecentChangesLinked/Fail-safe)
- [Special pages](https://en.wikipedia.org/wiki/Special:SpecialPages)
- [Permanent link](https://en.wikipedia.org/w/index.php?title=Fail-safe&oldid=1054345841)
- [Page information](https://en.wikipedia.org/w/index.php?title=Fail-safe&action=info)
- [Cite this page](https://en.wikipedia.org/w/index.php?title=Special:CiteThisPage&page=Fail-safe&id=1054345841&wpFormIdentifier=titleform)
- [Wikidata item](https://www.wikidata.org/wiki/Special:EntityPage/Q1392940)

### Print/export

- [Download as PDF](https://en.wikipedia.org/w/index.php?title=Special:DownloadAsPdf&page=Fail-safe&action=show-download-screen)
- [Printable version](https://en.wikipedia.org/w/index.php?title=Fail-safe&printable=yes)



### Languages

- [Deutsch](https://de.wikipedia.org/wiki/Fail-Safe)
- [فارسی](https://fa.wikipedia.org/wiki/شکست_امن)
- [Français](https://fr.wikipedia.org/wiki/Mode_dégradé)
- [Bahasa Indonesia](https://id.wikipedia.org/wiki/Konsep_gagal-aman)
- [日本語](https://ja.wikipedia.org/wiki/フェイルセーフ)
- [Русский](https://ru.wikipedia.org/wiki/Отказобезопасность)
- [中文](https://zh.wikipedia.org/wiki/失效安全)

[Edit links](https://www.wikidata.org/wiki/Special:EntityPage/Q1392940#sitelinks-wikipedia)

- This page was last edited on 9 November 2021, at 14:09 (UTC).