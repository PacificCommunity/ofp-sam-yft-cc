# Tasks

**YFT diagnostic run**

- Find the YFT diagnostic run folder
- Find the YFT diagnostic run script(s)
- Modify the YFT diagnostic run script(s)
- See if we can run the YFT diagnostic model
- Run the YFT diagnostic model with the old executable
- Run the YFT diagnostic model with the new executable

**Catch-conditioned model**

- Paste CC flags from SWO to YFT
- Share findings with Nick and get advice

**Plots**

- Read results into R

**Slides**

---

# Questions

1. The yellowfin diagnostic model doitall seems to stop between phases. When we
   run doitall for the first time, it creates 00.par and stops. If we run
   it again, it creates 01.par and stops. If we run it again, it starts phase 2.
   Is this the expected behavior, given the content of the script?

2. We have compared the swordfish 2017 refcase doitall and Nicks' swordfish CC
   solution phase file to isolate the CC flags. See:
   https://github.com/PacificCommunity/ofp-sam-mfcl-school/blob/main/tutorial_1_ccond/swo2017_arni/README.md.
   When we paste these CC flags into the yellowfin diagnostic model doitall and
   replace the original executable (2.0.7.0) with new (2.0.8.4 from 2022_02_23),
   we get the following error:

```
Making a copy of an unallocated dvector
Making a copy of an unallocated dvector
Making a copy of an unallocated dvector
making a copy of an unallocated age_length_record_array
Making a copy of an unallocated dvector
Making a copy of an unallocated dvector
Making a copy of an unallocated dvector
Making a copy of an unallocated dvector
 initial_tag_year(2) 194
Bounds error reading pmature(1) in par file
 value is 0
```
3. How do we enable the self-scaling multinomial to get appropriate sample size?

<!-- 4. The swordfish refcase doitall runs into an error in phase 10: line 296 if [] -->
