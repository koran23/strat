# Trading Strategy

This strategy focuses on specific time windows, top holder percentage levels, and strength/impact values to determine optimal trades.

---

## 1. Trading Window
- **Primary Window:** 7 PM – 10 AM  
  - The highest probability for successful trades occurs during this period.  
  - **Ignore** any trades or alerts outside this window.  

---

## 2. Top Holder Percentage
- **Target Range:** 0.005x – 0.006x  
  - All subsequent rules hinge on whether the top holder percentage is around **0.005** or **0.006**.  

---

## 3. Strength
- **Primary Reference:** 0.00000000  
  - Use this as a baseline for evaluating strength.  
- **Additional Strength Levels:**  
  - Determined by the **top holder percentage**.  
  - The examples below show specific values that have historically performed well (“SWEET SPOT”) or poorly (“DUD”).

### Example Strength Values

#### When Top Holder % = 0.005
- **20,566.63488546** – [DUD](https://dexscreener.com/solana/fswwhrbmzemnrgzfyyvtpj7ka9q9jsxqshd1in8akij4)  
- **34,369.12606089** – [SWEET SPOT – 4X](https://dexscreener.com/solana/63v5upzkhy5wgkdck1tmdkk4j3gtaw6ogxbsvdkqdrvz)  
- **59,878.07682169** – [SWEET SPOT – 9X](https://dexscreener.com/solana/dt273h3eojsdbjogrm1a6k93z8kiimhfarswagrq2grs)  
- **83,121.58805598** – [DUD](https://dexscreener.com/solana/68nqaun1ruwghzhzxuvnrbe5n6azqdhzzpzjokeqj4ph)

#### When Top Holder % = 0.006
- **208,143.52910098** – [SWEET SPOT – 10X](https://dexscreener.com/solana/bh3r92ql35eu7frqgfy6psy4lozdcojf4iazahuh73ad)

---

## 4. Impact Value
- **Check This Last** in every trade alert.  
- **Risk Thresholds:**  
  - At **0.005** top holder %, values near **20,000** can be risky.  
  - At **0.006** top holder %, values near **40,000** can be risky.

### Example Risky Impact Values

#### When Top Holder % = 0.005
- **21,232.46463921** – [DUD](https://dexscreener.com/solana/3iibjzxfuuuunpdd82vhsk7cb7yo7w92fvqh468rqptx)  
- **21,603.22273425** – [DUD](https://dexscreener.com/solana/qduzgd2fpnhclcstff3wl2ex47ywxgbcjtsk7ptpais)  
- **21,840.30920243** – [DUD](https://dexscreener.com/solana/ahyn5obpy6d4otddj4jbsdzqjgeqhvmh2jnjjjcnhmtt)  
- **26,239.77056979** – [DUD](https://dexscreener.com/solana/fswwhrbmzemnrgzfyyvtpj7ka9q9jsxqshd1in8akij4)

#### When Top Holder % = 0.006
- **42,821.31254038** – [DUD](https://dexscreener.com/solana/efl8uuwztg2kfyjphh4s9b6epiagw4vj3jwdgy8ecor4)  
- **44,141.21478593** – [DUD](https://dexscreener.com/solana/avqfgguyo8pp4rzunnvtklxvxpjddhjmjbcqwa9upr5a)

---

## 5. Transaction Filters
Use these filters to immediately **avoid** certain transactions based on the top holder percentage.

### If Top Holder % is around 0.005
- **Exclude** transactions showing impact values like:  
  - `3.78`, `4.x`, or `0.4x`

### If Top Holder % is around 0.006
- **Exclude** transactions showing impact values like:  
  - `3.78`

---

### Final Notes
1. **Focus on the correct time window (7 PM – 10 AM).**  
2. **Identify the top holder percentage (0.005 or 0.006) and use the respective strength, impact, and transaction filters.**  
3. **Check impact value last**—steer clear of values near the “risky” thresholds.
