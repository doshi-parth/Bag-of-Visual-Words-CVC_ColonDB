CVC-ColonDB

--------------------------------------------------
Introduction
--------------------------------------------------

CVC-ColonDB is a database of frames extracted from colonoscopy videos. 
These frames contain several examples of polyps. In addition to the frames, we provide the ground truth for the polyps. 
This ground truth consists of a mask corresponding to the region covered by the polyp in the image.

CVC-ColonDB has been generated from 15 different video studies. For each study a sequence containing a polyp was extracted. 
Finally, a set of frames were selected from each sequence, paying particular attention in showing several points of view of the polyp. 

--------------------------------------------------
Description
--------------------------------------------------

The database consists of three different types of images:
1) Original images: frame_number.tiff
2) Polyp masks: pframe_number.tiff
3) Polyp contour: cpframe_number.tiff

The correspondence between the number of frame and the video sequence is as follows: // TABLa

       ----------------------------------
       |                  |		|
       |   Frame Number   |   Sequence	|
       |                  |		|
       ----------------------------------
       |		  |		|
       |      1 to  38    |	 1	|
       |     39 to  60    |	 2	|
       |     61 to  76    |	 3	|
       |     77 to  97 	  |	 5	|
       |     98 to 148    |	 6 	|
       |    149 to 155    |	 7 	|
       |    156 to 203    |	 9	|
       |    204 to 208 	  |	10	|
       |    209 to 263    |	11	|
       |    264 to 273    |	14	|
       |    274 to 300    |	15	|
       |		  |		|
       |    301 to 320    |	4	|
       |    321 to 340    |	8	|
       |    341 to 360    |	12	|
       |    361 to 380    |	13	|
       ----------------------------------


CVC-ColonDB is the database used to generate the results published on Pattern Recognition
J.Bernal, J.Sánchez and F. Vilariño "Towards Automatic Polyp Detection with a Polyp Appearance Model", Elsevier.
The database used in the paper corresponds to frames 1 to 300.
Sequences 1,9 and 15 are especially rich in terms of number of different views of the polyp. 
Sequences 3 and 10 are short, they have few frames, and for this reason the number of different views is lower.

Sequence 4 presents fecal content. This makes difficult to provide a proper polyp mask.Sequence 8 also presents a lot of fecal content.
Sequence 12 has a bad quality of visualization of the polyp. Sequence 13 does not present frames with enough quality of point of view.

--------------------------------------------------
Referencing
--------------------------------------------------

If you use this database for your experiments please include the following reference:

Bernal, J., Sánchez, J. and Vilariño, F. ‘Towards automatic polyp detection with a polyp appearance model. Pattern Recognition. Volume 45, Issue 9, September 2012, Pages 3166–3182