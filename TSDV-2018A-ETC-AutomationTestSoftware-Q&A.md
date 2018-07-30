TSDV-2018A Automation Test Software Q&A list 
===
Revision history
---

|Rev. No.(X.YY)|Date(YY-MM-DD)|Section No. Changed|Change Description|Author|Reviewed by|Approved by|
|:---:|---|---|---|:---:|:---:|:---:|
0.01|2018-07-16|QnA|Add question QA001|LenLT|LanLTM|
0.02|2018-07-17 |QnA|Add answer QA0001|Nakayama|||
0.03|2018-07-16|QnA|Add question QA002|LanLTM||


---
Definitions
---

|No.|Acronyms|Definition|
|:---:|:---:|---|
|1|![afjahsdkfj](./image/New.png)       |Question is new        |
|2|![afjahsdkfj](./image/Discuss.png)   |Question is discussing |
|3|![afjahsdkfj](./image/Done.png)      |Question is done       |

---
<h2>List question</h2>

- [![](./image/Done.png) QA001: Simulate GUI of ETC Board and DSRC board](#-qa001-simulate-gui-of-etc-board-and-dsrc-board)
- [![](./image/New.png) QA002: Concern about version of simulator in the newest testing environment](#-qa002-concern-about-version-of-simulator-in-the-newest-testing-environment)

---
Question
---

## ![](./image/Done.png) QA001: Simulate GUI of ETC Board and DSRC board

**[2018-07-16][TSDV][LenLT]**

We have concern about simulating GUI of ETC Board and DSRC board.

**_1. ETC board_**

In document SM0004 [ETC処理部（ESE拡張基板）基本部ソフトウェア設計書.doc] section 4.3.8, 6 and 8, ETC board displays some error code in LED when executing testing.

**Do you want to simulate error code of LED in ETC software?**

**_2. DSRC board_**

DSRC board displays:
    * Status of Antenna
    * Status connection of DSRC board
    * Mode by dip switch: Maintenance mode, Testing mode,...
    
**Do you want to simulate status of antenna, connection and modes in DSRC Simulator?**

**[2018-07-17][TCSetsu][Nakayama]**

I'm sorry, I just recognize care about 7-segment. 
I think it's not necessary to emulate 7-segment, if we can check error code by operation in DSRC simulator.
Please consider a configuration and a log data for Dip-sw and 7-sagement.

## ![](./image/New.png) QA002: Concern about version of simulator in the newest testing environment

**[2018-07-30][TSDV][LanLTM]**

When we execute testing for accounting and fee check part in Japanese version of testing environment, we found that there are some problem:
    * Cannot execute testing continously
    * Sometime cannot reboot LS

So we concern about version of simulator in testing environment. Could you please confirm some points for us?
    * **Is there any change in RS sim and Kisetsu sim?** If yes, please share us the newest SRC of these simulators. We will modify these simulators to corresponding to testing software environment.
    * **Regarding ETC board, Do we need to upgrade ETC board?** If yes, please share us built file of ETCBoard to upgrade.
 