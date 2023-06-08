# Scene_recogintion
I started to make some changes on the original dataset (CVPR 09) the 
original dataset was 67 Indoor categories, and a total of 15620 images
So I removed the unwanted categories and the kind of duplicated categories 
and although I added new categories (e.g. mosque inside) at the end I had 
only 39 categories but decreasing the number of categories is not enough for 
sure, so I collected around +11K more picture then I cleaned those 
pictures to be only JPG.
Images then I filtered the data from all the bad paths images in the end I
had a new dataset with 26589 images belonging to 39 classes which names 
are :-
[auditorium, bakery , bathroom, bedroom, bookstore, children room, 
classroom, church inside, clothing store, concert hall, corridor, deli, dining 
room, fastfood_restaurant, florist, grocery store, gym, hair salon, hospital 
room, inside subway, kindergarten, kitchen, library, living room, lobby, mall, 
meeting room, nursery, office, pantry, pool inside, restaurant, staircase, shoe 
shop, toy store, waiting room, warehouse, laundry, inside mosque] 
For the first trial the validation accuracy didn't break the 55% on the other 
hand the training accuracy was + 80% which is a very huge gap and a low 
accuracy too.
After the new dataset I tried again, and we got a noticeable progress


I got + 60% validation accuracy and +95% training accuracy but still there is a 
gap between them (Over Fitting)…

After some research I found out that the most common dropout ratios are 
between 0.5, 0.8 and I was using a 0.25 dropout ratio so I started to 
train the model using 0.5, 0.75, 0.85, 0.8 and the best I could get so far is 0.8 
with the following results in Figure 33.

At the end we got Training accuracy 98.2% and a Validation accuracy 72.315%



