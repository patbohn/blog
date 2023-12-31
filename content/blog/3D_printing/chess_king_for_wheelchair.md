+++
title = "A Chess Piece that helps my dad control his electric wheelchair"
date = 2023-12-21
+++

## Intro 
What do you gift a person who is very limited in how they can move and where they can go? My mom and me have been thinking a lot about this while searching for Christmas presents for my dad (who has a slow-progressing form of ALS). And I think we found something: 

While my mom last met the technicians responsible for the maintenance of the electric wheelchair that my dad is using every day, they presented her with a 3D-printed skull as an attachment for the controller stick. While we were immediately excited about the general idea, we weren't sure about the skull theme. However, our thoughts shifted to something else: My dad has been playing chess since 4 decades (and is still actively playing!), so what could be better than a chess king as a controller stick?! Of course, requirements included it being haptic, providing a good grip, while not posing an injury risk. This made TPU the primary choice. 

So (as is tradition), I brought my 3D printer with me for this year's Christmas travel, along with a role of black TPU (95A) that I had already calibrated while printing some drone parts. This meant I could start printing immediately - which was great because it still took around 10 hours of total print time for the final gift. 

## The Design Process

I began by downloading an STL model for a [king chess piece from Creative-Prints](https://www.printables.com/model/582262-kingkonig-chess), imported it into Fusion 360, measured the inner diameter of the hole of a replacement rubber attachment, and incorporated such a hole to the model before started the first iteration of printing. After a few rounds of printing to evaluate the clearance for the hole diameter (decreasing it by 0.05 mm a few times) I finally achieved a good fit. (Tip: By printing out only the region of interest, for example by using the union setting of the Fusion 360 combine function, iteration speed is much faster while one saves material)

![picture](iterations_for_fit.jpg)

However, I wasn't entirely satisfied with the upper edge on the model, as both the print quality and haptics were suboptimal. Similarly, the cross on top didn't print well after reducing infill to 10% and perimeters to 2 (to minimize the risk of injury when falling into it). 

![prev_edge_overhang](prev_edge_overhang.jpg)

Therefore I decided to create my own model from sketch(es) in Fusion 360. 

To create my own model, I started with a sketch of the body. Here, I sketched the outline if the rotationally symmetric parts using arcs, ensuring they ended tangentially to a semi-circle to improve haptics and printability. I then created the body using the rotational extrusion function. 

![fusion_sketch](Fusion_sketch.png) 

To add the cross at the top I then created another sketch, again targeting improved printability by reducing the overhang angle at the bottom, and rounding out the edges a bit more. 

![fusion_fillets](Fusion_fillets.png)

Finally, I re-designed the cutout for the hole by adding small triangle extrusions to help gripping the metal pin of the electric wheelchair. And last but not least, during slicing I added a layer height modifier to reduce infill and perimeter number for the cross to ensure it is flexible. At a total print time of 65 minutes, I am quite proud how this turned out: 

## The Result

![mounted](final_mounted.jpg)

The final model is now [uploaded on Printables](https://www.printables.com/model/700548-chess-king-as-escooter-controller-stick-attachment), where I also have uploaded the tool models used to cut the hole. I hope this post may bring joy to someone else that is using such an electric wheelchair! 