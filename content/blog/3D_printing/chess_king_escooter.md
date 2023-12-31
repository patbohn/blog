+++
title = "A Chess King that helps my dad controlling his eScooter"
date = 2023-12-21
+++

## Intro 
What do you gift a person who's very limited in how they can move and where they can go? My mom and me have been thinking a lot about this when looking for christmas presents for my dad (who has a slow-progressing form of ALS) - and I think we found something: 

When my mom last met the technicians of the eScooter that my dad is using everyday, they presented her with a 3D-printed skull as an attachment for the controller stick. While we got immediately excited about the general idea, we weren't sure about the skull theme. However, our minds wandered to something else: My dad has been playing chess since 4 decades (and is still actively playing!), so what could be better than a chess king as a controller stick?! Of course, requirements included it being haptic, providing good grip, while not being an injury risk. This made TPU the primary choice. 

So (as is tradition), I took my 3D printer with me for this year's christmas travel, and with it a role of black TPU (95A) that I had calibrated already when printing drone parts. That meant I could start printing immediately - which was great because it still took around 10 hours of total print time for the final gift. 

## The Design Process

I started downloading an STL model for a [king chess piece from Creative-Prints](https://www.printables.com/model/582262-kingkonig-chess), imported it into Fusion 360, measured the inner diameter of the whole of a replacement rubber attachment, and added such a hole to the model, and started printing. After a few iterations on the hole diameter (decreasing it by 0.05 mm a few times) I think I found a good fit. (Tip: only printing out the region of interest, for example by generating a union (Fusion 360 combine function) helps a lot with iteration speed and saves material)

However, I wasn't quite happy yet with the upper edge on the model, as both the print quality and haptics were suboptimal. Similarly, the cross on top didn't print well after reducing infill to 10% and perimeters to 2 (to ensure no risk of injury when falling into it). So I decided to create my own model from sketch(es) in Fusion 360. 

To create my own model, I started with a sketch of the body. Here, I sketched the outline if the rotationally symmetric parts using arcs, ending tangentially to a semi-circle to improve haptics and printability. I then created the body using the rotational extrusion function. To add the cross at the top I then created another sketch, again targeting improved printability by reducing the overhang angle at the bottom, and rounding out the edges a bit more. Finally, I re-designed the cutout for the hole by adding small triangle extrusions to help gripping the metal pin of the eScooter. And last but not least, during slicing I added a layer height modifier to reduce infill and perimeter number for the cross to ensure it is flexible. At a total print time of 65 minutes, I am quite proud how this turned out: 

## The Result

The final model is now [uploaded on Printables](https://www.printables.com/model/700548), where I also have uploaded the tool models used to cut the hole. I hope this post may bring joy to someone else that is using such an eScooter! 