# Physical AI (フィジカルAI) Complete Benkyokai Script
**Topic:** Physical AI: Overview of Technologies & AI Concepts (技術とAI概念の概要)  
**Target Time:** ~18–20 Minutes

### Tips for Reading This Script
* **100% Pronunciation Ready:** Particles are written the way they are **pronounced** (`wa`, `o`, `e`) so you can read straight off the screen without tripping up.
* **Pacing (`/`):** Pause briefly at every `/` to take a breath and point at your slide.
* **Math & Technical Terms:** Written clearly so you can pronounce them naturally in Japanese katakana style or English.

---

## 1. 導入・Physical AIとは・発表の構成 (Introduction, What is Physical AI, & Presentation Structure) — [~3 mins]

**[Slide 1: Title Slide & Agenda]**

Minasan, konnichiwa. / Kyou wa, "Physical AI to, sore ni hitsuyou na gijutsu ya AI no gainen no gaiyou" ni tsuite happyou shimasu. / Yoroshiku onegaishimasu.

> *Hello everyone. Today, I will give a presentation on "Physical AI: An overview of the technologies and AI concepts needed for Physical AI." Thank you for having me.*

**[Slide 2: What People Think Physical AI Is vs. What It Actually Is]**

Mazu, "Physical AI" towa nan deshou ka? / Kantan ni iu to, "genjitsu no sekai o rikai shite, butsuri-teki ni ugoku AI" desu. / ChatGPT no you na AI wa, tekisuto ya gazou dake no sekai ni imasu. / Demo, Physical AI wa, kamera ya sensaa de genjitsu no sekai o mite, butsuri no housoku o rikai shimasu.

> *First, what is "Physical AI"? Simply put, it is "AI that understands the real world and acts physically." AI like ChatGPT exists only in the world of text and images. However, Physical AI looks at the real world with cameras and sensors, and understands the laws of physics.*

Ookuno hito wa, Physical AI to kiku to, "hitogata robotto" ya "jidou-unten no kuruma" dake o souzou shimasu. / Shikashi, jissai no Physical AI wa, sore dake dewa arimasen. / Robotto ya kuruma igai ni mo, takusan no rei ga arimasu.

> *When many people hear Physical AI, they only imagine "humanoid robots" or "self-driving cars." However, actual Physical AI is not just that. Even outside of robots and cars, there are many examples.*

Tatoeba, 1-tsume (hitotsume) wa, "Iryou ya Herusukea" desu. / Shujutsu o sapooto suru iryou shisutemu ya, byouin no kensa o jidou-ka suru shisutemu mo Physical AI desu. / 2-tsume (futatsume) wa, "Sumaato Biru ya Deeta Sentaa no Dejitaru Tsuin" desu. / Sensaa de heya no ondo ya kuuki no nagare o mite, eakon ya denryoku o jidou de chousei shimasu. / 3-tsume (mittsume) wa, "Kishou ya Denryoku Guriiddo no Dejitaru Tsuin" desu. / Chikyuu zentai no tenki ya, machi no enerugii o butsuri shimyureeshon de yosoku suru koto mo, Physical AI no ichibu desu.

> *For example, the first is "Medicine and Healthcare." Medical systems that support surgery and systems that automate hospital testing are also Physical AI. The second is "Digital Twins of Smart Buildings and Data Centers." Using sensors to monitor room temperature and airflow, AI automatically adjusts air conditioning and power. The third is "Digital Twins of Weather and Power Grids." Predicting global weather or city energy using physics simulations is also part of Physical AI.*

**[Slide 3: How This Presentation is Structured (The Single Running Example)]**

Koko de, kyou no happyou no kousei o setsumei shimasu. / Physical AI ni wa, 3D shimyureeshon kara AI no gakushuu made, totemo ooku no gijutsu ga arimasu. / Sorezore o bara-bara ni setsumei suru to, sukoshi wakari-nikui desu.

> *Here, I will explain the structure of today's presentation. In Physical AI, from 3D simulation to AI training, there are very many technologies. If I explain each one separately, it is a bit hard to understand.*

Desukara kyou wa, **1-tsu (hitotsu) no gutaiteki na purojekuto no rei** o tsukatte, subete no gijutsu to AI no gainen o setsumei shimasu. / Sono rei towa, **"Okyakusama no koujou (souko) no Dejitaru Tsuin o tsukuri, sono naka de AMR (Jiritsu Idou Robotto) o ugokasu"** to iu purojekuto desu. / Kyou shoukai suru NVIDIA ya Unity no tsuuru mo, AI no nyuuraru nettowaku ya saishin no moderu mo, subete "kono koujou to AMR no purojekuto de dou tsukau ka" to iu shiten de setsumei shite ikimasu.

> *Therefore, today, I will use **one concrete project example** to explain all the technologies and AI concepts. That example is a project where we **"build a Digital Twin of a customer's factory (or warehouse), and run an AMR (Autonomous Mobile Robot) inside it."** Both the NVIDIA and Unity tools I introduce today, as well as AI neural networks and the latest models, will all be explained from the perspective of "how we use them in this factory and AMR project."*

### Key Vocab (Section 1)
* **Gaiyou (概要):** Overview
* **Butsuri no housoku (物理の法則):** Laws of physics
* **Iryou (医療):** Medical care / Healthcare
* **Kousei (構成):** Structure (of the presentation)
* **Gutaiteki na rei (具体的な例):** Concrete example

---

## 2. デジタルツインの構築と2大エコシステム (Building the Digital Twin & The Two Main Ecosystems) — [~5 mins]

**[Slide 4: Why Do We Need a Simulator / Digital Twin First?]**

Mazu, okyakusama no koujou ni AMR o dousou (deploy) suru mae ni, naze shimyureeta ya dejitaru tsuin de AI o gakushuu saseru hitsuyou ga aru no deshou ka? / Omo na riyuu wa 3-tsu (mittsu) arimasu.

> *First, before deploying an AMR into a customer's factory, why do we need to train the AI in a simulator or digital twin? There are three main reasons.*

1-tsume (Hitotsume) wa, **"Anzen-sei" (Safety)** desu. / Koujou no naka ni wa, hataraite iru hito mo imasu shi, totemo takai kikai mo arimasu. / Mada gakushuu shite inai AMR o jissai no koujou de hashiraseru to, hito ya kikai ni butsukatte shimai, totemo kiken desu. / Dakara mazu wa, anzen na kasou kankyou ga hitsuyou desu.

> *The first is **"Safety."** Inside a factory, there are people working, and there are also very expensive machines. If we run an untrained AMR in an actual factory, it will crash into people or machines, which is very dangerous. So first, we need a safe virtual environment.*

2-tsume (Futatsume) wa, **"Koujou o tomerarenai" (Cannot stop the factory)** koto desu. / AI no gakushuu ya tesuto no tame ni okyakusama no koujou no rain o tomeru to, totemo ookina keizai-teki na sonshitsu (economic loss) ni narimasu.

> *The second is that **"We cannot stop the factory."** Stopping the customer's factory line for AI training or testing results in huge economic losses.*

3-tsume (Mittsume) wa, totemo juuyou desu ga, **"Heiretsu de daikibo na tesuto ga dekiru" (Massive parallel testing)** koto desu. / Honmono no AMR 1-dai (ichi-dai) dake de gakushuu suru to, nan-shuukan mo kakarimasu. / Demo, shimyureeta no naka nara, nan-zen-dai (thousands) mono AMR o douji ni (in parallel) hashiraseru koto ga dekimasu. / Kore ni yotte, AI no gakushuu ga totemo hayaku shuusoku (converge) shimasu.

> *The third—and very important—reason is that **"We can do massive testing in parallel."** If we train with only one real AMR, it takes many weeks. However, inside a simulator, we can run thousands of AMRs simultaneously in parallel. Because of this, the AI training converges much faster.*

**[Slide 5: A Digital Twin is NOT Just a 3D Model + Development Flow]**

Koko de daiji na pointo wa, **"Dejitaru Tsuin wa, tada no 3D moderu dewa nai"** to iu koto desu. / Dejitaru Tsuin ni wa, juuryoku ya yuka no masatsu (friction) nado no **butsuri keisan** ga arimasu. / Soshite, LiDAR ya kamera nado no **sensaa no shimyureeshon** mo arimasu.

> *An important point here is that **"A Digital Twin is not just a 3D model."** A Digital Twin has **physics calculations** like gravity and floor friction. And it also has **sensor simulations** like LiDAR and cameras.*

Sarani, okyakusama no **jissai no sagyou kankyou (actual working environment)** o sono mama saigen shimasu. / Tatoeba, koujou no naka o aruku sagyousha (workers) ya, hoka no ugoku robotto mo dejitaru tsuin no naka ni iremasu. / Baai ni yotte wa, jissai no koujou kara riarutaimu de deeta o okuri, ima no koujou to hotondo onaji joutai o konpyuuta no naka ni tsukurimasu.

> *Furthermore, it reproduces the customer's **actual working environment**. For example, workers walking inside the factory and other moving robots are also placed inside the digital twin. Depending on the case, we send data in real time from the actual factory, creating a state inside the computer that is almost identical to the current real factory.*

Kono purojekuto o tsukuru nagare to, kiso gijutsu no tsukaikata wa kou desu:
1. Mazu, doroon (drone) ya 3D sukyanaa o tsukatte, okyakusama no koujou o sukyan shimasu.
2. Sono koujou no 3D deeta o, **"OpenUSD"** to iu kyouyuu keishiki de hozon shimasu.
3. Tsugi ni, AMR no kansetsu ya taiya no kouzou o kaita **"URDF"** deeta o koujou ni iremasu.
4. Saigo ni, **"ROS 2" (DDS ya Zenoh)** no tsuushin o tsukatte, kasou no AMR to seigyo sofutowea o tsunagimasu. (ROS to OpenUSD wa izen no benkyokai de shoukai sareta node, shousai wa shouryaku shimasu.)

> *The flow of building this project and how foundational technologies are used is like this:*
> *1. First, using drones or 3D scanners, we scan the customer's factory.*
> *2. We save that factory's 3D data in a shared format called **"OpenUSD."***
> *3. Next, we put the **"URDF"** data—which describes the AMR's joints and tire structure—into the factory.*
> *4. Finally, using **"ROS 2" (DDS or Zenoh)** communication, we connect the virtual AMR to the control software. (Since ROS and OpenUSD were introduced in a previous study meeting, I will skip the details.)*

**[Slide 6: Ecosystem 1 — NVIDIA Physical AI Stack]**

Kono koujou to AMR no dejitaru tsuin o tsukuru tame no, 2-tsu (futatsu) no ookina ekoshisutemu ga **"NVIDIA"** to **"Unity"** desu. / Mazu, NVIDIA no tsuuru ga kono purojekuto no doko o tsukuru ka setsumei shimasu.

> *The two major ecosystems for building this factory and AMR digital twin are **"NVIDIA"** and **"Unity."** First, I will explain which part of this project each NVIDIA tool builds.*

* **NVIDIA Omniverse:** OpenUSD o beesu ni shita 3D no dodai (foundation) desu. Sukyan shita okyakusama no koujou o koko ni tsukuri, hikari no hansha ya butsuri (PhysX) o keisan shimasu.
* **NVIDIA Isaac Sim:** Omniverse no ue de ugoku robotto-you shimyureeta desu. AMR ni kasou no LiDAR ya kamera o tsukete, ROS 2 to tsuushin sasemasu.
* **NVIDIA Isaac Lab:** AI o gakushuu saseru tame no tsuuru desu. Koujou no naka de nan-zen-dai mono AMR o douji ni ugokashite, AI o kunren (train) shimasu.
* **NVIDIA Cosmos:** Kore wa "World Foundation Model" (Sekai Kiban Moderu) desu. Koujou no 3D eizou kara, yuka ga nurete iru joutai ya, kurai joutai nado, honmono sokkuri no eizouバリエーション (variations) o jidou de tsukurimasu. / **Kono World Foundation Model to eizou seisei ni tsuite wa, ato no AI no paato de mou ichido kuwashiku setsumei shimasu.**

> * **NVIDIA Omniverse:** The 3D foundation based on OpenUSD. We build the scanned customer factory here and calculate light reflections and physics (PhysX).
> * **NVIDIA Isaac Sim:** The robot simulator running on Omniverse. It attaches virtual LiDAR and cameras to the AMR and connects it to ROS 2.
> * **NVIDIA Isaac Lab:** The tool for training AI. It runs thousands of AMRs in parallel inside the factory to train the AI.
> * **NVIDIA Cosmos:** This is a "World Foundation Model." From the factory's 3D video, it automatically creates photorealistic visual variations, like wet floors or dark lighting. **We will come back to World Foundation Models and this photorealistic video generation in more detail later in the AI part of this presentation.**

**[Slide 7: Ecosystem 2 — Unity Physical AI Stack]**

Tsugi ni, **Unity** no ekoshisutemu de onaji koujou purojekuto o tsukuru baai desu. / Unity wa dousa ga karukute, UI ya VR o tsukuru no ga totemo tokui desu.

> *Next is when we build the same factory project using the **Unity** ecosystem. Unity runs lightly and is very good at creating UIs and VR.*

* **Unity Engine:** Koujou no 3D kuukan o ugokashi, koujou no kanri gamen (dashboard) ya, VR de robotto o sousa suru gamen o tsukurimasu.
* **Unity Simulation Pro (SimPro):** Robotto senyou no atarashii pakkeeji desu. URDF de AMR o yomikomi, LiDAR ya kamera o tsukete, ROS 2 to高速 (kousoku) ni tsuushin shimasu. Kuraudo (Cloud) de takusan no shimyureeshon o mawasu koto mo dekimasu.
* **Unity ML-Agents & Sentis:** **ML-Agents** wa, Unity no naka de AMR no AIエージェント (agent) o gakushuu saseru kankyou desu. Soshite **Sentis** wa, gakushuu shita AI moderu o Unity no naka de chokusetsu ugokasu tsuuru desu.

> * **Unity Engine:** Runs the 3D factory space and builds the factory management dashboard or VR robot teleoperation screens.
> * **Unity Simulation Pro (SimPro):** A new package dedicated to robotics. It imports the AMR via URDF, attaches LiDAR and cameras, and communicates at high speed with ROS 2. It can also run many simulations in the cloud.
> * **Unity ML-Agents & Sentis:** **ML-Agents** is the environment for training the AMR's AI agent inside Unity. And **Sentis** is the tool that runs the trained AI model directly inside Unity.

### Key Vocab (Section 2)
* **Keizai-teki na sonshitsu (経済的な損失):** Economic loss
* **Heiretsu (並列):** Parallel
* **Shuusoku suru (収束する):** To converge (training finishes)
* **Jissai no sagyou kankyou (実際の作業環境):** Actual working environment
* **Saigen suru (再現する):** To reproduce / replicate

---

## 3. AIの基礎知識：AI・機械学習・ディープラーニング (AI Fundamentals: AI, ML, DL, & RL) — [~3 mins]

**[Slide 8: Diagram of AI > Machine Learning > Deep Learning + RL]**

Koko kara wa, koujou no AMR no "Atama (Brain)" ni naru **AI no paato** ni hairimasu. / Watashitachi no busho dewa AI kaihatsu o chokusetsu shite inai node, mazu wa AI no kiso kara kantan ni setsumei shimasu.

> *From here, we will enter the **AI part**, which becomes the "Brain" of our factory AMR. Since our department does not directly do AI development, I will first briefly explain the fundamentals of AI.*

Surido no zu (diagram) o mite kudasai.
* Ichiban ookii waku ga **"AI (Jinkou Chinou)"** desu. / Mukashi kara aru `if-else` no ruuru-beesu no puroguramu mo koko ni hairimasu.
* Sono naka ni aru no ga **"Machine Learning (Kikai Gakushuu)"** desu. / Ningen ga ruuru o kaku kawari ni, konpyuuta ga deeta kara ruuru o manabimasu.
* Sarani sono naka ni aru no ga **"Deep Learning (Shinsou Gakushuu)"** desu. / Ningen no nou (brain) o maneta "Nyuuraru Nettowaku" o tsukatte, kamera no eizou ya 3D deeta nado no fukuzatsu na jouhou o shori shimasu.

> *Please look at the diagram on the slide.*
> * *The largest circle is **"AI (Artificial Intelligence)."** Traditional `if-else` rule-based programs are also included here.*
> * *Inside that is **"Machine Learning."** Instead of humans writing rules, the computer learns rules from data.*
> * *Further inside that is **"Deep Learning."** Using "Neural Networks" that imitate the human brain, it processes complex information like camera video and 3D data.*

**[Slide 9: Supervised, Unsupervised, and Reinforcement Learning in the Warehouse]**

Machine Learning to Deep Learning no naka ni wa, omo ni **3-tsu (mittsu) no gakushuu houhou** ga arimasu. / Koujou no AMR no rei de mite mimashou.

> *Inside Machine Learning and Deep Learning, there are mainly **three learning methods**. Let's look at them using our factory AMR example.*

1. **Supervised Learning (Kyoushi-ari Gakushuu):** "Kotae (Answer)" ga aru deeta de manabu houhou desu. / Tatoeba, ningen ga "Kore wa hito", "Kore wa fookurifuto" to namae (label) o tsuketa koujou no shashin o nan-man-mai mo misete, AMR no kamera ni shougai-butsu (obstacles) o oboesasemasu.
2. **Unsupervised Learning (Kyoushi-nashi Gakushuu):** "Kotae" ga nai deeta kara, AI ga jibun de pataan (patterns) o mitsukeru houhou desu. / Tatoeba, AMR no motaa no oto ya shindou (vibration) no deeta dake o misete, "itsumo to chigau koshou no maebure (anomaly)" o jidou de guruupu-wake sasemasu.
3. **Reinforcement Learning / RL (Kyouka Gakushuu):** Zu no naka de Deep Learning to kasanatte iru (overlapping) totemo daiji na gijutsu desu. / Kotae o oshieru kawari ni, dejitaru tsuin no naka de AMR ni "Shikou-sakugo (trial and error)" o sasemasu. / Mokutekichi ni tsuitara **Purasu 10-ten (+10 points)**, kabe ni butsukattara **Mainasu 50-ten (-50 points)** to iu **Houshuu (Reward)** o ataeru koto de, AMR wa jibun de jouzu na hashirikata o manabimasu.

> *1. **Supervised Learning:** Learning from data that has an "Answer key." For example, we show tens of thousands of factory photos where humans labeled "This is a person" or "This is a forklift," teaching the AMR's camera to recognize obstacles.*
> *2. **Unsupervised Learning:** A method where AI finds patterns by itself from data without answers. For example, by showing only motor sound and vibration data from the AMR, it automatically groups "unusual signs of a breakdown."*
> *3. **Reinforcement Learning (RL):** A very important technology overlapping with Deep Learning in the diagram. Instead of teaching the answer, we make the AMR do "trial and error" inside the digital twin. By giving a **Reward**—such as **+10 points** for reaching the goal and **-50 points** for hitting a wall—the AMR learns how to drive well by itself.*

### Key Vocab (Section 3)
* **Jinkou Chinou (人工知能):** Artificial Intelligence (AI)
* **Kikai Gakushuu (機械学習):** Machine Learning (ML)
* **Shinsou Gakushuu (深層学習):** Deep Learning (DL)
* **Kyoushi-ari / Kyoushi-nashi (教師あり / 教師なし):** Supervised / Unsupervised
* **Kyouka Gakushuu (強化学習):** Reinforcement Learning (RL)
* **Houshuu (報酬):** Reward

---

## 4. ニューラルネットワークの仕組みと学習プロセス (How Neural Networks Work & The Training Process) — [~4 mins]

**[Slide 10: Inside a Neural Network — Neurons, Weights, and Biases]**

Tsugi ni, Deep Learning no chuushin de aru **"Nyuuraru Nettowaku" (Neural Network)** ga dou natte iru no ka, mou sukoshi kuwashiku mite mimashou.

> *Next, let's look in a bit more detail at how a **"Neural Network,"** which is at the center of Deep Learning, is structured.*

Nyuuraru Nettowaku wa, watashitachi **ningen no nou (human brain)** no kouzou o参考にして (sankou ni shite) tsukuraremashita. / Ningen no nou ni wa, **"Nyuuron" (Neuron)** to iu chiisana saibou (cells) ga takusan arimasu. / Onaji you ni, AI no Nyuuraru Nettowaku mo, konpyuuta no naka no chiisana **"Nyuuron"** ga takusan tsunagatte deきて imasu.

> *A Neural Network was created inspired by the structure of our **human brain**. In the human brain, there are many tiny cells called **"Neurons."** In the same way, an AI's Neural Network is made of many tiny digital **"Neurons"** connected together inside a computer.*

Dewa, kono 1-tsu (hitotsu) no dejitaru na nyuuron no naka ni wa, nani ga haitte iru deshou ka? / Jitsu wa totemo shinpuru de, **"Weight (Omomi)"** to **"Bias (Baiasu)"** to iu 2-tsu (futatsu) no suuji (numbers) dake desu. / Shiki de kaku to, $y = w \cdot x + b$ no you na kantan na keisan desu.

> *So, what is inside one of these digital neurons? Actually, it is very simple: there are only two numbers, called **"Weight"** and **"Bias."** Written as a formula, it is a simple calculation like $y = w \cdot x + b$.*

* **"Weight (Omomi)" ($w$) towa:** Haitte kita jouhou ($x$) ga, "dorekurai juuyou ka" o kimeru suuji desu. / Tatoeba, AMR ga hashitte iru toki, "tenjou no iro (ceiling color)" wa amari kankei arimasen node, Weight wa chiisaku ($0.01$ nado ni) narimasu. / Demo, "1-meetoru mae ni hito ga iru" to iu LiDAR no jouhou wa totemo juuyou na node, Weight wa ookiku ($0.99$ nado ni) narimasu.
* **"Bias (Baiasu)" ($b$) towa:** Sono nyuuron ga "dono kurai hannou shiyasui ka" no kijun-chi (threshold / offset) desu. / Nyuuryoku ni tasizan sareru kihon no suuji desu.

> * **What is a "Weight" ($w$)?** It is a number that decides "how important" an incoming piece of information ($x$) is. For example, when an AMR is running, the "color of the ceiling" doesn't matter much, so its Weight becomes small (like $0.01$). However, LiDAR information saying "there is a person 1 meter ahead" is very important, so its Weight becomes large (like $0.99$).*
> * **What is a "Bias" ($b$)?** It is the baseline threshold (offset) that decides "how easily that neuron reacts/fires." It is a base number added to the input.*

**[Slide 11: Forward Pass, Loss Function, Backward Pass, & RL Reward-to-Loss]**

Saishin no ookina AI moderu ni wa, kono nyuuron ga **nan-oku-ko (billions)** mo haitte imasu. / Saisho wa, subete no nyuuron no Weight to Bias wa detarame (random) na suuji desu. / Kore o "Gakushuu 루ープ (Training Loop)" de sukoshi-zutsu (little by little) chousei shimasu.

> *In modern large AI models, there are **billions** of these neurons. At first, the Weights and Biases of all neurons are random numbers. We adjust them little by little using the "Training Loop."*

1. **Forward Pass (Jun-denpan):** Mazu, AMR ga kamera no eizou o mite, ima no Weight to Bias de keisan shi, koudou o yosoku shimasu (tatoeba, "migi ni magaru").
2. **Loss Function (Sonshitsu Kansuu):** Tsugi ni, sono koudou ga "dono kurai machigatte ita ka" o suuji (Loss / Error) ni shimasu.
   * *Kyouka Gakushuu (RL) no baai:* AMR ga kabe ni butsukatte **Mainasu 50-ten (-50 reward)** o moratta to shimasu. / Shisutemu wa, kono "moratta Houshuu (Reward)" to "kitai shite ita Houshuu" no sa o keisan shite, **Loss Function (machigai no ookisa)** ni henkan shimasu. / Tsumari, "Houshuu ga hikui = Loss (machigai) ga ookii" to keisan sareru wake desu.
3. **Backward Pass (Gyaku-denpan / Backpropagation):** Kono Loss (machigai) no jouhou o, nyuuraru nettowaku no ushiro kara mae e gyaku-houkou ni nagashimasu. / Soshite, nan-oku-ko mo aru nyuuron no Weight to Bias o **honno sukoshi dake (tatoeba $0.001$ dake)** kakikaemasu.

Kore o dejitaru tsuin no naka de nan-byaku-man-kai mo kurikaesu koto de, nan-oku-ko no nyuuron ga sukoshi-zutsu chousei sare, saigo ni wa watashitachi ga hoshii tadashii kekka (butsukarazu ni hashiru AMR) ni **shuusoku (converge)** shimasu.

> *1. **Forward Pass:** First, the AMR looks at the camera image, calculates using its current Weights and Biases, and predicts an action (for example, "turn right").*
> *2. **Loss Function:** Next, it turns "how wrong that action was" into a score (Loss / Error).*
>    * *In the case of Reinforcement Learning (RL):* Suppose the AMR hits a wall and gets a **-50 reward**. The system calculates the difference between this "received Reward" and the "expected Reward," converting it into a **Loss Function (size of the mistake)**. In short, "Low Reward = High Loss."*
> *3. **Backward Pass (Backpropagation):** This Loss information is sent backward from the end of the neural network to the front. Then, it rewrites the Weights and Biases of the billions of neurons **just a tiny bit (for example, by $0.001$)**.*
> *By repeating this millions of times inside the digital twin, the billions of neurons are adjusted little by little, and finally they **converge** toward the exact result we want (an AMR that drives without crashing).*

**[Slide 12: Training Problems (Under/Overfitting) & Transfer Learning / Fine-Tuning]**

Kono gakushuu dewa, 2-tsu (futatsu) no yoku aru mondai ni ki o tsukeru hitsuyou ga arimasu.
* **Underfitting (Gakushuu-busoku):** Gakushuu ga tarinai joutai desu. AMR wa shimyureeta no naka demo mada massugu hashiremasen.
* **Overfitting (Ka-gakushuu):** Gyaku ni, shimyureeta no koujou no kabe no iro ya hako no ichi o **anki (memorize)** shite shimau mondai desu. / Shimyureeta dewa 100-ten desu ga, jissai no koujou de sukoshi shoumei (lighting) ga kawaru dake de, AMR wa ugokenaku narimasu.

> *In this training, we need to watch out for two common problems:*
> * **Underfitting:** A state where training is insufficient. The AMR still cannot even drive straight inside the simulator.*
> * **Overfitting:** Conversely, the problem where the AI **memorizes** the exact wall colors and box positions of the simulator factory. It gets 100% in the simulator, but if the lighting changes slightly in the real factory, the AMR stops working.*

Sokode, jissai no purojekuto dewa **"Transfer Learning (Ten'i Gakushuu)"** to **"Fine-Tuning (Fain Chuuningu)"** o tsukaimasu. / Zero kara AI o tsukuru no dewa naku, mazu wa ippan-teki na koujou no dejitaru tsuin de kiso o gakushuu sasemasu (Pre-training). / Soshite saigo ni, **okyakusama no koujou no tokubetsu na deeta** (okyakusama dake no nimotsu no katachi ya yuka no iro) o sukoshi dake tsukatte, Weight o saishuu chousei (**Fine-Tuning**) shimasu. / Kore nara, sukunai deeta to mijikai jikan de okyakusama senyou no AI ga dekimasu.

> *Therefore, in real projects, we use **"Transfer Learning"** and **"Fine-Tuning."** Instead of building AI from scratch, we first train the basics in a general factory digital twin (Pre-training). Then finally, using a small amount of **data specific to the customer's factory** (the customer's unique box shapes or floor colors), we do a final adjustment (**Fine-Tuning**) of the Weights. This way, we can create a customer-specific AI with little data and in a short time.*

### Key Vocab (Section 4)
* **Ningen no nou (人間の脳):** Human brain
* **Omomi / Weight (重み):** Weight ($w$)
* **Kijun-chi (基準値):** Threshold / Baseline (Bias $b$)
* **Sonshitsu Kansuu (損失関数):** Loss Function
* **Sukoshi-zutsu (少しずつ):** Little by little
* **Ka-gakushuu (過学習):** Overfitting

---

## 5. Physical AIの最新トレンド：基盤モデル (The Current Frontier: Foundation Models for Physical AI) — [~3.5 mins]

**[Slide 13: The Paradigm Shift — LLMs/VLMs & VLA Models]**

Tsugi wa, ima sekai de ichiban chuumoku sarete iru **Physical AI no Foundation Models (Kiban Moderu)** ni tsuite desu. / Kore made wa, "kamera de miru AI", "michi o kimeru AI" no you ni, chiisana AI o bara-bara ni tsukutte imashita. / Demo ima wa, 1-tsu (hitotsu) no ookina AI ga subete o rikai suru **"Hanyou Robotto Nou (Generalist Robot Brain)"** ni kawatte kite imasu. / Omo ni 3-tsu (mittsu) no shurui ga arimasu.

> *Next is about **Foundation Models for Physical AI**, which are getting the most attention in the world right now. Until now, people built small, separate AIs—like "an AI for looking with a camera" and "an AI for choosing a path." But now, it is shifting toward a **"Generalist Robot Brain,"** where one large AI understands everything. There are mainly three types.*

1-tsume (Hitotsume) wa, **"LLM to VLM (Vision-Language Models)"** o keikaku (High-Level Planner) ni tsukau houhou desu. / Tatoeba, koujou no maneejaa ga AMR ni mukatte, *"3-ban no tsuuro (Aisle 3) ni koboreta mizu o souji shite"* to kotoba de iimasu. / Suruto VLM wa kamera to kotoba o rikai shite, *"1. Tsuuro 3 ni iku -> 2. Mizu o mitsukeru -> 3. Souji suru"* to iu chiisana tasuku ni bunkai (Task Decomposition) shi, ROS 2 ni meirei o okurimasu.

> *The first is using **"LLMs and VLMs (Vision-Language Models)"** as High-Level Planners. For example, a factory manager says to the AMR in natural words, "Clean up the spilled water in Aisle 3." Then the VLM understands the camera and words, breaks it down (Task Decomposition) into small sub-tasks—"1. Go to Aisle 3 -> 2. Find the water -> 3. Clean it"—and sends the commands to ROS 2.*

2-tsume (Futatsume) wa, **"VLA Models (Vision-Language-Action)"** desu. / Kore wa VLM o sarani shinka saseta mono desu. / Kamera no eizou (Vision) to ningen no kotoba (Language) o ireru to, AI ga chokusetsu **Robotto no Koudou (Action)**—tatoeba taiya no sokudo ya robotto aamu no $(x, y, z)$ no ichi—o dasu End-to-End no moderu desu. / Yuumei na rei toshite wa, Google no **RT-2**, **OpenVLA**, Physical Intelligence no **$\pi_0$ (Pai-Zero)**, soshite NVIDIA no **Project GR00T** ga arimasu.

> *The second is **"VLA Models (Vision-Language-Action)."** This takes VLMs one step further. When you input camera images (Vision) and human words (Language), it is an end-to-end model where the AI directly outputs **Robot Actions**—such as wheel speed or a robot arm's $(x, y, z)$ coordinates. Famous examples include Google's **RT-2**, **OpenVLA**, Physical Intelligence's **$\pi_0$ (Pi-Zero)**, and NVIDIA's **Project GR00T**.*

**[Slide 14: World Foundation Models (WFMs) & Synthetic Video Generation]**

3-tsume (Mittsume) ga, saisho no NVIDIA no paato de sukoshi fureta **"World Foundation Models (Sekai Kiban Moderu)"** desu. / Kore wa, nan-zen-만-jikan mono genjitsu no douga (video) o gakushuu shite, **juuryoku (gravity), masatsu (friction), mono no ugoki ya mizu no nagare** nado, "kono sekai no butsuri no ruuru" o rikai shite iru AI desu.

> *The third is **"World Foundation Models,"** which I briefly touched on earlier in the NVIDIA part. This is an AI trained on tens of millions of hours of real-world video so that it understands the "physical rules of this world," such as **gravity, friction, object permanence, and fluid dynamics**.*

Koujou no AMR purojekuto dewa, omo ni 2-tsu (futatsu) no tsukaikata ga arimasu:
1. **Mirai no Yosoku (Future Prediction):** AMR ga "Moshi kono nimotsu o oshitara, kuzureru ka na?" to, koudou suru mae ni atama no naka de mirai o yosoku suru tame ni tsukaimasu.
2. **Gousei Douga no Seisei (Synthetic Video Generation):** Genzai tsukaeru daihyou-teki na gijutsu ga, NVIDIA ga happyou shita **"NVIDIA Cosmos"** to, sono **Gousei Douga Seisei Tsuuru (Cosmos Transfer / Omniverse Replicator)** desu. / Tatoeba, dejitaru tsuin de tsukutta shinpuru na 3D no koujou douga o Cosmos ni ireru dake de, AI ga jidou-teki ni "ame no hi", "yoru no kurai koujou", "yuka ga yogorete iru koujou" nado, honmono no shashin no you na (photorealistic) nan-zen-bon mono gakushuu-you douga ni henkan shite kuremasu. / Kore ni yotte, jissai no koujou de shashin o toranakute mo, mugen ni AI no gakushuu deeta o fuyasu koto ga dekimasu.

> *In our factory AMR project, there are mainly two ways to use it:*
> *1. **Future Prediction:** The AMR uses it to predict the future in its head before acting, asking, "If I push this stack of boxes, will it fall over?"*
> *2. **Synthetic Video Generation:** The representative technologies available right now are **"NVIDIA Cosmos"** and its **Synthetic Video Generation tools (Cosmos Transfer / Omniverse Replicator)** launched by NVIDIA. For example, just by feeding a simple 3D factory video from our digital twin into Cosmos, the AI automatically transforms it into thousands of photorealistic training videos—"a rainy day," "a dark factory at night," or "a factory with dirty floors." Because of this, even without taking photos in the real factory, we can infinitely expand our AI training data.*

### Key Vocab (Section 5)
* **Kiban Moderu (基盤モデル):** Foundation Model
* **Bunkai suru (分解する):** To decompose / break down
* **Yosoku (予測):** Prediction
* **Gousei Douga (合成動画):** Synthetic Video

---

## 6. Sim-to-Realの壁とまとめ (Crossing the Sim-to-Real Gap & Conclusion) — [~2.5 mins]

**[Slide 15: Crossing the "Sim-to-Real Gap" & Edge Deployment]**

Saigo no gijutsu-teki naテーマ (theme) wa, **"Sim-to-Real" (Shimyureeshon kara Genjitsu e)** desu. / Dejitaru tsuin de AI o gakushuu saseta ato, sono AI o honmono no AMR ni ireru to, umaku ugoite kurenai koto ga yoku arimasu. / Kore o **"Sim-to-Real Gap"** to yobi, Physical AI o yaru kigyou ni totte ichiban ookina kadai (challenge) no hitotsu desu.

> *The final technical theme is **"Sim-to-Real" (from Simulation to Reality)**. After training an AI in a digital twin, when you put that AI into a real AMR, it often fails to work properly. This is called the **"Sim-to-Real Gap,"** and it is one of the biggest challenges for companies working in Physical AI.*

Naze nara, shimyureeta wa "kirei sugiru" kara desu. / Genjitsu no okyakusama no koujou ni wa, yuka no abura (oil) ni yoru suberi, kamera no ranzu no hikari no hansha (glare), soshite tsuushin no okure (latency) ga arimasu.

> *This is because simulators are "too clean." In a customer's real factory, there is wheel slipping from oil on the floor, light glare on camera lenses, and communication latency.*

Kono kabe (gap) o koeru tame ni, enjinia wa **"Domain Randomization (Domein Randamuka)"** to iu gijutsu o tsukaimasu. / Dejitaru tsuin de AMR o gakushuu saseru toki ni, wazato (intentionally) yuka no suberi-yasusa, nimotsu no omosa, hikari no tsuyosa, sensaa no noizu o maikai randamu ni kaemasu. / Suruto AI wa, donna kankyou no henka ni mo tsuyoi (robust) nou ni sodachimasu. / Soshite saigo ni, sono AI moderu o chiisaku karuku shite (Quantization / TensorRT), AMR no naka ni aru chiisana konpyuuta (Edge GPU) ni irete, genba de ugokashimasu.

> *To cross this gap, engineers use a technique called **"Domain Randomization."** While training the AMR in the digital twin, we intentionally and randomly change the floor slipperiness, payload weight, light brightness, and sensor noise every single time. Then the AI grows into a brain that is robust to any environmental change. Finally, we compress the AI model to make it small and fast (Quantization / TensorRT), load it onto the onboard computer (Edge GPU) inside the AMR, and run it at the real site.*

**[Slide 16: Conclusion — Why This Matters for Our Team]**

Saigo ni, kyou no matome desu. / Kyou wa, koujou to AMR no dejitaru tsuin o rei ni shite, Physical AI no shimyureeshon kankyou (NVIDIA to Unity) kara, Nyuuraru Nettowaku no shikumi, soshite VLA ya World Foundation Model made, zentai no nagare o shoukai shimashita.

> *Finally, here is today's summary. Today, using the factory and AMR digital twin as an example, I introduced the entire flow of Physical AI—from simulation environments (NVIDIA and Unity), to how Neural Networks work, to VLAs and World Foundation Models.*

Watashitachi no chiimu mo kore kara Physical AI no bunya (domain) ni haitte iku naka de, kono bunya ni donna tsuuru ya gijutsu ga aru no ka, zentai-zou (the big picture) o shitte oku koto wa totemo juuyou da to omoimasu. / Kyou hanashita subete no gijutsu o ima sugu fukaku (at deep depth) shiranakute mo, **"watashitachi ga tsukaeru donna tsuuru ya AI gijutsu ga aru ka"** to iu kiso chishiki (fundamental knowledge) o motte ireba, kore kara atarashii Physical AI no purojekuto ga kita toki ni, tadashii gijutsu o erande sumuuzu ni sutaato dekiru to omoimasu.

> *As our team enters the Physical AI domain from now on, I think it is very important to know the big picture of what tools and technologies exist across this entire domain. Even if we don't know every technology discussed today at deep depth right away, if we have the fundamental knowledge of **"what tools and AI technologies are at our disposal,"** when we come across a new Physical AI project in the future, we will be able to choose the right technologies and start smoothly.*

Watashi no happyou wa ijou desu. / Go-seichou arigatou gozaimashita. / Nanika shitsumon wa arimasu ka?

> *That concludes my presentation. Thank you very much for listening. Are there any questions?*

---

## Bonus: Handy Survival Phrases for Q&A (質疑応答用フレーズ)
1. **Thanking them for the question:**
   * *Shitsumon arigatou gozaimasu.* (Thank you for the question.)
2. **Asking them to repeat it slowly:**
   * *Sumimasen, mou ichido, yukkuri itte itadakemasu ka?* (Excuse me, could you say that one more time slowly?)
3. **Switching to English if the answer is technical:**
   * *Chotto fukuzatsu na node, eigo de kotaete mo ii desu ka?* (Since it's a bit complex, is it okay if I answer in English?)
4. **If you don't know the answer:**
   * *Sumimasen, soko wa mada kuwashiku shirabete inai node, ato de kakunin shimasu.* (Sorry, I haven't researched that part in detail yet, so I will check it later.)