---
title: "Automatic Carassius Auratus Feeder with Water Changer Mechanism (ACAFWWCM)"
description: "A developmental research project designing a low-cost, automated system to care for goldfish by combining precise daily feeding schedules with an automated water filtration and changing mechanism."
publishDate: 2023-05-15
tags: ["Research", "Hardware Prototype", "Arduino", "Automation"]
img: "/ck-website/assets/works/thesis.jpg"
featured: false
---
## Introduction

No one is prepared for the Corona virus (COVID-19) pandemic outbreak. There are many things changed ever since it began. People face the realities of physically disconnecting or isolating themselves from their friends or social ties and remaining home 24/7 with nothing else to do. Then comes the trends such as online selling, TikTok application, planta/tito, or petting different animals. This research developed a device to help fish owners care for their pets, especially goldfish. Any home would benefit from having a goldfish aquarium or tank. Because goldfish require much space to roam, their number must be considered. A larger tank is needed for a single-tailed goldfish or more than one beautiful goldfish. Pet owners should be able to keep their goldfish healthy and strong. They should be knowledgeable about growing beneficial bacteria in their tank and setup the correct filtration and lighting [1].

This project designed a low-cost device that allows goldfish enthusiasts to care for their fish more effectively without as much work and exertion. The owner can trust the device to look after their goldfish in a manner that ensures its care. Overfeeding is one of the most common causes of goldfish death. When the food in the tank decomposes, the proteins release ammonia and nitrites, reducing the tank’s oxygen quantity. Lack of oxygen in the water harms the fish, especially the goldfish. This can be difficult for fish owners who need to leave the house but need a reliable pet sitter. While there are several alternatives for feeding cats and dogs while away from home, there are fewer options for fish owners.

Goldfish have a daily feeding schedule, which makes it difficult for the fish owner to be away from home, whether for school, business, or pleasure. This necessitates the development of an automated device capable of feeding a goldfish reliably.

This research details the group's process to design, build, and test an Automatic Goldfish Feeder with Water Changing Mechanism. The researchers came up with the idea to develop an automated device with a water changing device to ensure the cleanliness of the water in the aquarium even without the owner and a goldfish feeder to dispense the accurate amount of food into the aquarium at a particular time each day. This project may help lessen the owner's worries for their goldfish if they are not home because they can rely on the device to perform its function.

## Related Works

This chapter offers national and international literature that discusses characteristics, aptitudes, and technological advancements related to the prototype. Researchers with both direct and in direct relations to the project are also included.

### Benefits of Fish Feeder
This automatic fish feeder can be set up as often throughout the day as the fish require. These are basic machines that only require providing food and setting a timer. [2] The fact that owners do not need to be there to feed their fish is the main advantage of an automatic fish feeder. Fish should receive food from the automatic fish feeder. If the fish is fed multiple times a day and cannot or does not want to feed them by hand, this automated feeding is helpful for several days [2]. The pet fish owners are usually distressed when they are away from the home environment because they cannot feed the fish on time. When away from home, pet fish owners are frequently upset because they cannot feed the fish on time. Food deprivation and overfeeding put fish health at risk and lower the water quality in indoor fish tanks. Therefore, keeping an eye on the fish feeder is crucial and can benefit owners [3]. [4] A standard fancy goldfish should consume around 2% of its body weight daily. A small 20-gram fish would need 2% of its weight, or 0.4grams, throughout the day. The researchers developed a fish feeder for fish pellets; the amount of food stored inside the fish feeder container is small.

### Automatic Water Changer
Water replacement is one of the most crucial aspects of aquarium maintenance. Regular aquarium water changes are necessary to maintain fish health and avoid unpleasant, dark water. Owners can eliminate extra nutrients that can adversely affect their fish tank environment when they remove filthy aquarium water from their fish tank and replace it with clean, freshwater. Constantly replenish trace elements supporting the tank's residents' well-being and enjoying a stunning underwater environment. [5] The aquarium may experience a wide range of problems due to in frequent water changes. Skipping water changes can cause problems for the fish and other marine inhabitants, creating an unattractive, uncomfortable, and smelly aquarium. It is crucial to be aware that changing the water in the aquarium can affect its chemistry and nutrient potential.

Meanwhile, corals are constantly utilizing and depleting these resources to stay alive. Use clean seawater or a quality saltwater aquarium mix to replenish any vital components removed to the appropriate levels [illusions]. Some nutrients and organics, such as phosphates and nitrate, irritating the aquarium residents, are also removed when draining some aquarium water. The interior of the tank will be vulnerable to algae grow that high phosphate and nitrate concentrations, and the health and development of the fish will also be impacted.

### Importance of Water Quality
Water is essential for maintaining life. Marine life requires equal attention for clean environment. The impurities in an existing aquarium threaten the life of the marines. As a result, fish could not survive and could die as well, and also, for existing aquariums removing impurities from water in the aquarium is a crucial issue. They regularly test water quality parameters, such as turbidity sensors, to measure the number of suspended particles in the water [6].

Turbidity is a measurement of how cloudy or murky water is. Turbidity increases with water cloudiness. Submerged Aquatic Vegetation (SAV), receive less sunlight when there is a high turbidity level. Because plants create oxygen, fewer plants grow, which limits the amount of oxygen available to aquatic life. Low sunlight penetration is caused by high turbidity.

High turbidity damages fish habitat, jams fish gills, and makes water unfit for drinking. Significant amounts for aquatic animals and plants: (a) a turbidity meter is used to measure turbidity. Aquatic life is harmed by turbidity levels above 150 NTUs at any given time or 50 NTUs monthly. (b) A Secchi disk is used to gauge the clarity of the water. Turbidity can block gills and prevent fish from seeking food when the disk cannot be seen below 1 meter [7].

## Methodology

This chapter describes the research methodology employed in the study. It also includes illustrations that help to visualize the prototype's process. The project design, development, instruments, and procedures will be described.

### A. System Flow
Figure 1 shows the system's overview and step-by-step process. The Arduino board is the microcontroller of the system and the one responsible for sending and getting data from the other components and storing all the commands that will perform by the device. The device is activated when power from an outlet through the Arduino is supplied. It will automatically read the set time at the predetermined periods for feeding the goldfish and changing the water. Then it will compare the predetermined feeding and water-changing times for the goldfish.

If the device is powered on, the program will begin running; it will use the LCD to show the programmed designs and visuals on the screen. The fish feeder will produce a goldfish meal if the set time is met. Another feature is the turbidity sensor. It will run if the sensor detects the murky and unclear water and automatically filters it using the pump. The manual feeder and water changer mechanism buttons are an additional benefit. These benefits allow the user to engage and manually operate the device. The water changer mechanism is utilized if the sensor determines that the water is dirty or if the button for the changer is pressed. Two water pumps will start pumping the water into the aquarium from a reserve water container when activated.

<div class="grid grid-cols-1 md:grid-cols-2 gap-4 my-6">
  <div class="text-center">
    <img src="/ck-website/assets/works/system-flow.png" alt="System Flow" class="mx-auto rounded-lg shadow-md max-h-80" />
    <p class="text-sm italic mt-2">Fig. 1. System Flow Diagram</p>
  </div>
  <div class="text-center">
    <img src="/ck-website/assets/works/system-flowchart.png" alt="System Flowchart" class="mx-auto rounded-lg shadow-md max-h-80" />
    <p class="text-sm italic mt-2">Fig. 2. System Flowchart</p>
  </div>
</div>

### System Layout
Figure 3 depicts the devices' physical connection. The automatic timer set through the program determines the precise day and time the fish feeder and water changer device runs. It is also connected to the Arduino that controls the system and other mechanisms. The input device, such as the tactile buttons, is the manual control for the fish feeder and water filter.

The output devices are a fish feeder, water changer, and LCD screen display. The LCD screen display provides the visuals for the results of the programmed device. The fish feeder and water changer mechanism are connected to the microprocessor. The scheduled time is the access to the automatic features. The Arduino's analog, input, and output pins control the turbidity sensor. The purpose of the relay is to control the pump in filtering the water. The pump pulls the water into the designed filter.

<div class="text-center my-6">
  <img src="/ck-website/assets/works/layout.png" alt="System Layout and Overview" class="mx-auto rounded-lg shadow-md max-w-lg" />
  <p class="text-sm italic mt-2">Fig. 3. System Layout & Prototype Overview</p>
</div>

### Fabrication of the Prototype
Details, functionalities, and images of the finished item's real structural components were included. The researchers either took the images included here or properly cited internet images.

The Automated Feeder, Filter, and Turbidity Sensor comprise the following structural components: automatic feeder's housing, filter, and circuit storage case. The aquarium is placed with all materials and parts attached. The feeder’s box has a dimension of 0.42 ft. x 0.75 ft. It is also portable, removable, and simple to install in any kind of aquarium. Furthermore, affixed to the front of the case are the LCD and the buttons.

<div class="text-center my-6">
  <img src="/ck-website/assets/works/frontview.jpeg" alt="Front view of the fish feeder’s actual prototype" class="mx-auto rounded-lg shadow-md max-w-lg" />
  <p class="text-sm italic mt-2">Fig. 4. Front view of the fish feeder’s actual prototype</p>
</div>

The feeder's housing, cylinder support canister, funnel, and feeds holder are all plastic. The cylinder support canister holds the device's first feature, which is the automatic fish feeder. It also includes a funnel inside to ensure it will not jam when the servo motor spins to open, and the fish food will be fed to the goldfish. The servo motor is placed below the funnel to receive the feeds as it spin from 0 to 180 degrees. The researchers applied blue spray-paint to represent the essence of fish and an aquarium.

<div class="text-center my-6">
  <img src="/ck-website/assets/works/insideview.jpg" alt="Inside view of the fish feeder’s actual prototype" class="mx-auto rounded-lg shadow-md max-w-lg" />
  <p class="text-sm italic mt-2">Fig. 5. Inside view of the fish feeder’s actual prototype</p>
</div>

While the filter for the water changing mechanism is housed in a plastic container, the filter container at the top of the aquarium is fiber acrylic. Pumice, crushed lava, activated carbon, lava rings, and ceramic rings are used in the water-changing mechanism filter to help cleanse the water. Ceramic rings, lava rings, pepper balls, pumice, and foams are on the filter at the top of the aquarium.

<div class="grid grid-cols-1 md:grid-cols-3 gap-4 my-6">
  <div class="text-center">
    <img src="/ck-website/assets/works/filter.jpg" alt="Filter and Water Change Mechanism 1" class="mx-auto rounded-lg shadow-md max-h-60" />
  </div>
  <div class="text-center">
    <img src="/ck-website/assets/works/filter2.jpg" alt="Filter and Water Change Mechanism 2" class="mx-auto rounded-lg shadow-md max-h-60" />
  </div>
  <div class="text-center">
    <img src="/ck-website/assets/works/filter3.jpg" alt="Filter and Water Change Mechanism 3" class="mx-auto rounded-lg shadow-md max-h-60" />
  </div>
</div>
<p class="text-sm italic text-center mt-2">Fig. 6. Filter for the aquarium and water changer mechanism</p>

### Creating the Program’s Code

Using the Arduino microcontroller board, the researchers could write software that would run on the device. The source code portion of the appendices contains examples of the produced codes. The researchers created all of the device's codes—from initialization to starting title, turbidity reading, feeder and filter counts, manual feeding and filtering, automation system timers, and system fusion.

## Conclusions and Future Works

The study aimed to create an automatic goldfish feeder with a water-changer mechanism using an Arduino UNO and evaluate its effectiveness. Based on the research findings, the developed device can improve the care and maintenance of goldfish aquariums. The fact that the feeder and filter pumps can be controlled manually or according to a predetermined schedule, gives the user flexibility and convenience. The programmable turbidity sensor ensures that the water quality is maintained in the desired range, improving the health and well-being of the goldfish. The fish feeder, which releases a measured amount of feed daily, prevents overfeeding and minimizes waste. The water changer mechanism, which uses a recirculation system, helps preserve water and decrease the need for frequent water changes. The device's effectiveness was assessed by determining whether it operates according to the prescribed schedule or time. The results indicate that the device is reliable and functions as intended.

In conclusion, creating an automatic goldfish feeder with a water-changer mechanism using an Arduino Uno is an innovative idea with the potential to enhance the quality of life for both goldfish and their owners. Further research and development could lead to an even more advanced and effective automated aquarium maintenance system.

For further development of the device the researchers suggests to add a feature that recognizes and adjusts to each fish species’ unique traits and behaviors. Although the current prototype can operate manually and automatically, it is advised to upgrade the device by adding a wireless connection to support additional gadgets like smart phones and tablets to solve this problem. With the integration of voice recognition technology, users would no longer have to click the device physically, as they could use voice commands to operate it. It is essential to consider the other parameters that need to be controlled to maintain a healthy and optimal environment for fish.