# OPENRESP-V1

Open Resp (Nisshash)


FIGHT AGAINST COVID-19

 
UI INPUT
TIDAL VOLUME (Vt)
RESPIRATORY RATE(RR)
INHALE TO EXHALE RATIO(I:E)
OXYGEN CONCENTRATION CONTROL (FI02)

SAFETY ADDON:
1)PEAK PRESSURE ALARM
2) PEEP LEVEL DETECTION
3) PATIENT BREATHING DETECTION
4) SAFE FOR INTUBATED INVASIVE TYPE VENTILATION and also Noninvasive type CPAP mode
SPECIAL ADDON :
1)	SELF TEST ON STARTUP
2)	INLET OXYGEN DETECTION
3)	INHALE EXHALE FLOW RATE DETECTION
4)	TEMPERATURE DETECTION

KEY DIFFERENCE
COST 15000 BDT




Features:
1.	Only concentrated for Covid-19 patients who required  ICU and perform sedated intubating and providing ventilation including Clinical steps taken for ARDS ensuring all safety and alarm required by any medical authority global.
2.	UI of the machine similar of existing commercial machine.
3.	Standard industrial component wick are widely available but robust quality low cost have been us.  
4.	No kind of mold is necessity ( if not emphasized  on beutification )  mold needs initial investment and one to two month lead time depending on complexity.
5.	Deliberately mold biggest in size so or excessive shill is required assemble it in confined space.
6.	Components selected such a way that they are easily and accurately assembled by unshelled and uneducated man and woman just loading into assembly picture step.
7.	 Assembly tools requires very minimal and easily available in Bangladesh.
8.	Control system used widely available at mega 2560 chip and shields used for normal 3d printer
9.	Power system used normal laptop charger battery which is widely available
10.	3d Printed parts are very small and very fast to print, Single 3d printer can print all required parts for 5 device in a day.
11.	Laser cutter is widely available in all over the country. Laser cutter parts can be made in a day for 20 device. If laser cutter is not available by pasting paper print on PVC sheet manually can be cut with a grinder and a drill
12.	GE make ambo bag and ventilator circuit is used which is widely recommended by doctors and Chinese one is known to be leased or failed and this one is disposable. Reusable type ambo bag also can be used as the clamp is made universal for any type available.

13.	Most component have alternative type. As for example if lead screw is not found threaded rod can be used if stepper motor is short in only geared motor can be used with hall effect sensor with minor modification of the code.
14.	For mechanical movement guide part we did not choose square rail block or smooth rod linear lubrication and prone to rusting in unit condition and also very expensive. We used normal 625zz volar bearing (which is widely available) with a POM rubber or tips printed cover assembled as D wheel. Guided on aluminum profile which also serve as a rigid frame of the moving system.

15.	 We did not used fancy sensor few reasons 
a.	Bangladesh has no single manufacturer and due to COVID-19 situation worldwide international sourcing from USA, Japan even China is uncertain, lengthy and expensive.
b.	Fancy Sensors have reality issue if not used properly. So they are always needs a redundancy which means more cost

Key Innovations:
1.	Pressure sensor alternative:  Our observation is Ambu bag is a good replication of the Ling that it is connected to, when due to obstacle in air way passage or deterring Lung compliance the stiffness of the ambo bag increased. It means stepper motor would require move torque to push stiffer lung fora a given amount of travel. More torque means more current. So stiffer (or Pressure) can be translated in to motor input current by motor drive. 
Now question is, is this a new invention? Answer is No. 

Trinamic motor drive made by trinamic Germany (or the very available Chinese clone) can detect and directly control motor current. How we know it? Or have we used it? Yes. Because we make our own 3d printer. And sensor less honing and crash detection already solved years ago by many other 3d printer companies on of which is popular prusa I3 MK3. So what is our plan? 
Lung Compliance decrease


Ambu bag stiffness increase


Trinamic detects the current i. e force


Conversion to pressure (with a calibrated conversion table) 

Cons:
Only cons of this system is it is required
1. Intelligent coding which uses nothing but brain process
2. Lab our for calibration with standard pressure sensor both are manageable.

Problem and Solution: This will not be a instantaneous detection but a delay of few ms so on set peak pressure (Peak) the controller will provide alarm on Peak x 0.95 level 



Redundancy 1: As a complete independent redundancy a peak pressure relief valve with a pre- set pressure will be used in conjunction of the system.



Redundancy 2: As we will use two motor, so two TMS driver will be used. So naturally both driver can detect stiffness via current and act as a redundancy or fail safe each other So when reliability halter air is flowed on the plate it will suddenly change its resistance and we can amplify the signal to converts it to flow, It can easily detect flow or no flow, can detect flow rate rise or fall with adequate accuracy (±10%). So it can be used as a failsafe or a alternative calibration component a. 

2.	Flow Sensor alternative: We can easily incorporate flow sensor in our design. But still did not as application area is Bangladesh or similar country where a reliable supply chain of special flow sensor has its own risk, time and cost. So we also have to check for a reliable alternative. 
Component a) As we can detect stiffness, we can easily calibrate the volume VS motor distance travel under a given stiffness. And easily make a calibration table which can be easily verified with a flow sensor and also with air displacement volume under water. On a final device that table or a 3-parameter fitted equation can be used to predict flow rate and calculate tidal volume. Error of the system can be minimized very much as it will be compared to two independent tests. One a flow sensor two a volume level.
Component B) We will use a very basic wheatstone bridge and a industrially widely used PT 100 sensor to detect temperature to resistance change. 
On a platinum wire used inside a PT100 placed on an aluminum sink plate are very sensitive of temperature change and normally we test it by blowing air over it. 

Component B problem and solution: Heating and Cooling of PT100 platinum wire has one limitation which is a time lag of signal it can be easily overcome by making zero flow limit detection level shifted positively by 5%. So on 5% it will detect no flow and combined with current detection which is highly sensible it can trigger next logic. 


