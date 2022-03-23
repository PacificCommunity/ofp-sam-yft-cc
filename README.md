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
   When we paste these CC flags into the yellowfin diagnostic model doitall, we
   get the following error:
   ```
   icount = 7
   icount = 7
   icount = 7
   Fish not conserved -- Excess fishing mortality penalty =
   1.5766052167337300e+12
   Avoided move
   this option not implemented for implicit catchability
   ```

3. How do we enable the self-scaling multinomial to get appropriate sample size?

<!-- 4. The swordfish refcase doitall runs into an error in phase 10: line 296 if [] -->
