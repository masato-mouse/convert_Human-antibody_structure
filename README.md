# antibody-assesment

Summary 

mouse-antibody convert human-antibody with BioPhy.  
And use Alphafold2, contribute mouse-antibody structure and human-antibody structure.  

method

① access SabDab(http://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) and choose mouse-antibody   
② access BioPhy(https://biophi.dichlab.org/) and choose Humanize  
③ copy and paste VH and VL of mouse-antibody to BioPhy-Humanize from you choose mouse-antibody on SabDab  
④ select Humanaization setting and Humaness evaluation setting.　you finished , click 「submit」  
   (my favorite setting is iteration:5 and Humanaize CDRs)  
⑤ express result, click 「show aligment」  
⑥ copy and save converted VH and VL  
⑦ access PDB() and reseach mouse-antibody   
⑧ select FASTA Sequence in Display files  and copy FASTA Sequence  
⑨ copyed FASTA sequence rewrite VH and VL(⑥)  
⑩ access Alphafold2 and insert rewrite Sequence  

-> you will show human-antibody structure


