# Hadith Transmission Network in Kutub al-Arba'a

An interactive network visualization of 232 influential hadith transmitters, selected based on the volume of their narrations in the four primary Shia hadith collections (Kutub al-Arba'a).

## 📊 Data Source
The data was gathered manually using the **Dirayat al-Noor** software program.

## ⚙️ Layout Methodology
* **Initial Version:** The layout was manually set. 
* **Current Version:** The nodes are distributed using Gephi's "Ordered Graph Layout". The X-axis is based on ForceAtlas, and the Y-axis is based on the transmitter's Year of Death.
* [View the initial version here](https://www.academia.edu/11293931/گراف_اسناد_کتب_اربعه).

## 🎨 Visual Legend

### Node Color: Reliability Grade of the Narrator
* 🟡 **Yellow:** معصوم (Imams)
* 🟢 **Green:** جلیل (Eminent)
* 🔵 **Blue:** ثقه (Trustworthy)
* ⚪ **Gray:** مهمل (Unrated)
* 🟠 **Orange:** ضعیف (Weak)

### Node Size: Number of Narrations
The size class equals the number of digits in the narrator’s narration count.
* **Size 5** : >10,000 .
* **Size 4** : >1,000.
* **Size 3** : >100.

### Edges (Lines)
Each edge links a narrator to the authority he narrated from, and every Imam is the authority at the end of his edges.

**Line Thickness:** Shows the number of narrations carried by the chain, on the same digit scale as node size:
* **5:** (thickest): 10,000 or more
* **4:** 1,000–9,999
* **3:** 100–999
* **2:** 10–99
* **1:** (thinnest): 1–9

**Line Style:**
* **Solid lines:** Chains drawn mainly from the Four Books, using Dirayat al-Noor software.
* **Dashed lines:** Chains taken from the fihrist and rijal works (Najashi, Tusi’s Fihrist, Kashshi).

## 📋 Selection Criteria

### Narrator Inclusion
A narrator is included if he has any of the following:
* More than 300 hadiths, with at least 50 of them from two shaykhs.
* More than 500 hadiths.
* More than 100 hadiths narrated directly from an infallible.

### Chain Inclusion
A chain is shown only if both of its ends are included. Additionally:
* A chain must account for more than 5–10% of the narrator’s hadiths or more than 10–20% of the narrated-from’s hadiths.
* Chains between two ends must cover at least 50% of their shared narrations, counting unnamed narrators at the head of the list, and 25% without them.
* Chains from an Imam must carry more than 10–20 distinct narrations.

*Note: These limits were relaxed where long paths would have overcrowded the page.*

## 🛠️ Credits & Templates
* The visualization template was provided by the [InteractiveVis project](http://blogs.oii.ox.ac.uk/vis/).
