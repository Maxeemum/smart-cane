# smart-cane
A smart cane that tracks recovery progress by measuring force exerted over time.

![Smart Cane](./photos/IMG_7320.jpeg)

**Smart Cane Project**

In the summer of 2024, during recovery from ACL reconstruction surgery, the idea emerged to create a tool that could assist others facing similar challenges. A smart cane that helps users monitor their recovery by tracking the force they apply while using it. As recovery progresses, users should exert less force on the cane, indicating improved strength and mobility. This real-time feedback provides valuable insight, helping individuals stay motivated and on track with their recovery goals.

**Design and Prototyping**

Drawing from prior experience with Arduino, I was able to identify the right approach for measuring force, which led to the discovery of load cells—devices that convert mechanical strain into electrical signals. A wooden prototype was constructed, incorporating load cells into the handle. Initial designs encountered challenges in attaching the load cells securely while maintaining their functionality.
Elastic bands were used to hold the load cells in place, enabling accurate stress measurement. The [HX711](https://github.com/RobTillaart/HX711) repository was used to process data from the load cells, and zero the scale to account for the elastic bands' force.

**Electronics and Integration**

The load cells were connected using a Wheatstone bridge circuit and linked to an Arduino. To power the system, a battery pack was added. However, a need was identified for a memory module to store data for long-term tracking.
At this point my recovery progressed to the point where I could walk fine on my own so I shelved the project, but had it been completed, I would assume the following image is how the data would look.

![Smart Cane](./photos/recoveryplot.png)

**Future Development** <br>
Planned improvements for the next iteration include:
- **Memory Storage**: Incorporating a module to save recovery data over time.
- **Enhanced Design**: Developing a more ergonomic and durable cane.
- **Bluetooth Connectivity**: Adding wireless functionality to sync data with a companion app, enabling visualization of recovery progress and additional metrics like heart rate.
- **Monetization**: Offering a subscription-based app with advanced analytics and tracking features for users.

