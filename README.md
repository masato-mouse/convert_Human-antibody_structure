# convert Human-antibody structure

## Summary 

mouse-antibody convert human-antibody with BioPhy.  
And use Alphafold2, contribute mouse-antibody structure and human-antibody structure.  

## method

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

you will show human-antibody structure
And you can see it antigen and human-antibody by after step

11 get antigen with SabDab
12 get ginna and do it

→ you will show human-antibody structure


## example

I click 「search structure」 and 「search structiure by attribute」on SabDab.  
![スクリーンショット 2022-05-29 1 (3)](https://user-images.githubusercontent.com/85027378/170834080-f81fbe05-35c8-4616-b7d9-afb76d689bd2.png)　　



I click 「species : MUS MUSCULUS」and 「get Structure」.
![スクリーンショット 2022-05-29 1 (1)](https://user-images.githubusercontent.com/85027378/170834035-117dc5ab-48d5-440b-ad4d-6c92e247621f.png)

I select 1JP5 and copy Heavy chain and light chain on A/A.  
![スクリーンショット 2022-05-29 1 (2)](https://user-images.githubusercontent.com/85027378/170834007-7f734b9c-c691-45a4-881d-3738cd2ac0be.png)



copy and save Heavy chain Sequence and light chain Sequence after convert Heavy chain and light chain with BioPhy.  
![スクリーンショット 2022-05-29 2](https://user-images.githubusercontent.com/85027378/170836148-46c61581-13fb-4c40-b271-c0eb193c9297.png)
![スクリーンショット 2022-05-29 1 (4)](https://user-images.githubusercontent.com/85027378/170836150-82d7d0a6-bf7c-42c6-bff5-416022bf0b9c.png)



access PDB and reseach 1JP5.  
click and save FASTA Sequence.  





convert 
<mouse_Heavy chain Sequence　→ Human_Heavy chain Sequence> 
EVQLQQSGPELKKPGETVKISCKATNYAFTDYSMHWVKQAPGGDLKYVGWINTETDEPTFADDFKGRFAFSLDTSTSTAFLQINNLKNEDTATYFCVRDRHDYGEIFTYWGQGTTVTVSS  
↓  
QVQLVQSGSELKKPGASVKVSCKASGYTFTSYAMHWVRQAPGQGLEWMGWINTNTGNPTYAQGFTGRFVFSLDTSVSTAYLQISSLKAEDTAVYYCARDRHDYGEIFDYWGQGTLVTVSS  

<mouse_light chain Sequence → Human_light chain Sequence>  
DILMTQTPLYLPVSLGDQASISCRSSQTIVHNNGNTYLEWYLQKPGQSPQLLIYKVSNRFSGVPDRFSGSGSGTDFTLKISRVEAEDLGIYYCFQGSHFPPTFGGGTKLEIK  
↓  
DIVMTQTPLSLPVTLGQPASISCRSSQSLVHSNGNTYLYWYLQKPGQSPQLLIYKVSNRFSGVPDRFSGSGSGTDFTLKISRVEAEDVGVYYCMQGLHFPPTFGQGTKVEIK


<1JP5 mouse_all Sequence>
<span style="color: green">DILMTQTPLYLPVSLGDQASISCRSSQTIVHNNGNTYLEWYLQKPGQSPQLLIYKVSNRFSGVPDRFSGSGSGTDFTLKISRVEAEDLGIYYCFQGSHFPPTFGGGTKLEIK</span>GGGGSGGGGSGGGGS<span style="color: red">EVQLQQSGPELKKPGETVKISCKATNYAFTDYSMHWVKQAPGGDLKYVGWINTETDEPTFADDFKGRFAFSLDTSTSTAFLQINNLKNEDTATYFCVRDRHDYGEIFTYWGQGTTVTVSS</span>

<1JP5 human _all Sequence>
<span style="color: green">DIVMTQTPLSLPVTLGQPASISCRSSQSLVHSNGNTYLYWYLQKPGQSPQLLIYKVSNRFSGVPDRFSGSGSGTDFTLKISRVEAEDVGVYYCMQGLHFPPTFGQGTKVEIK</span>GGGGSGGGGSGGGGS<span style="color: red">QVQLVQSGSELKKPGASVKVSCKASGYTFTSYAMHWVRQAPGQGLEWMGWINTNTGNPTYAQGFTGRFVFSLDTSVSTAYLQISSLKAEDTAVYYCARDRHDYGEIFDYWGQGTLVTVSS</span>



last, use Alphafold2, express Human-antibody Structure.
(alphafpld2 URL:https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb)
insert human_all Sequence 

mouse-antibody-1JP5 with alphafold2
<img width="643" alt="スクリーンショット 2022-06-05 22 44 23" src="https://user-images.githubusercontent.com/85027378/172167764-2fc07372-64c2-42f1-9caf-dbf536eaf3d8.png">

human-antibody-1JP5 with alphafold2
<img width="638" alt="スクリーンショット 2022-06-05 23 27 19" src="https://user-images.githubusercontent.com/85027378/172167933-5ea520ab-b2c5-48e1-ae7b-8cc598bdcec2.png">


AND get antibody.pdb by SaBDAB













