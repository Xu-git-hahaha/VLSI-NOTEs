**光刻技术的两个领域**，在商业制造中实现**高通量生产**和**低成本大规模复制**的重要性。

光刻技术分为两个主要阶段：

1.  **初始图案生成 (Initial pattern generation)**：
    *   目标：创建微米级和纳米级图案的初始副本。
    *   方法：“所有尖锐的‘笔’绘图技术都是串行写入 - 逐点、逐线地绘制图案 - 这是一个非常缓慢的过程”。 这暗示了早期的或某些类型的光刻技术可能使用类似笔绘的方式，逐点逐线地创建图案。 这种方法虽然可以精确地创建初始图案，但效率很低，速度慢。

2.  **图案复制 (Pattern replication)**：
    *   目标：低成本、高通量地复制初始副本（称为母版）。
    *   优势：实现大规模生产，降低成本，提高效率。
    *   重要性：“对于商业制造，我们需要并行图案化能力以实现高通量生产”。  “如果我们没有低成本的大规模复制技术，集成电路芯片的价格可能会非常昂贵”。 这说明了图案复制技术对于降低集成电路成本，实现商业化生产至关重要。


**母版 - 光掩模 & 能量束图案绘制**

**一、母版 (Master Copy) - 光掩模 (Photomask)**

*   也称为光掩模 (Photomask)。
*   构成：玻璃板 (glass plate) + 铬 (Chrome) 图案。
*   玻璃 (Glass)：透明 (transparent to light)。
*   铬 (Chrome)：阻挡光线传播 (block light transmission)。
*   作用：大规模复制微纳米图案的母版。

**二、能量束 (Energy Beams) “笔”绘制图案**

*   能量束类型：电子束 (electron beam) 或 光子束 (photon beam)。
*   中间层：光刻胶 (Resist)。
    *   对光子能量/电子能量敏感。
    *   曝光后，化学结构变化 -> 溶剂溶解度改变。
    *   类似于照片底片，能量束改变其性质。

**三、通用光刻流程 (General Schemes)**

1.  **能量束曝光：**
    *   操纵能量束，在光刻胶层上扫描/曝光预定图案。

2.  **溶剂显影：**
    *   浸泡光刻胶层于溶剂中。
    *   **正性光刻胶：**  去除曝光区域。
    *   **负性光刻胶：**  保留曝光区域，去除未曝光区域。
    *   结果：光刻胶层形成图案。

3.  **图案转移 - 刻蚀：**
    *   以光刻胶图案为掩模 (mask)。
    *   使用刻蚀技术 (etching technique) 将图案转移到基底 (substrate)。
    *   刻蚀去除无光刻胶保护的基底材料。
    *   最终在基底上复制光刻胶图案。
![image](https://github.com/user-attachments/assets/ee7ae3c3-db10-480a-bfb5-94520b69f627)


**光刻胶 (Resists for Energy Beam Lithography)**

*   **能量束作用:** 电子束或光子束可以改变聚合物材料的链结构。

*   **正性光刻胶 (Positive resist):**
    *   **曝光区域：**  聚合物链断裂 (Chain scission)。
    *   **溶解性：**  断裂后更易溶于弱溶剂。
    *   **显影后效果：**  曝光区域被去除，留下未曝光区域图案。

*   **负性光刻胶 (Negative resist):**
    *   **曝光区域：** 聚合物链交联 (Cross-link)。
    *   **溶解性：** 交联后更难溶于弱溶剂。
    *   **显影后效果：** 曝光区域被保留，去除未曝光区域图案。

*   **光刻胶配方：**  光刻和电子束光刻有很多不同的光刻胶配方（化学成分）。

<img width="593" alt="image" src="https://github.com/user-attachments/assets/99579ffa-8e46-4c5e-bf93-2644eb23a40e" />

**光刻技术 (Lithography)**  以及它在 **集成电路制造 (IC layout)** 中的应用。

*   **光刻的定义：** 光刻是一种在 **基底 (substrate)** 上 **创建 (create) 和复制 (replicate) 图案** 的工艺。

*   **光刻的目的：**
    *   在基底表面（例如硅晶圆）上 **创建图案**，这些图案 **定义了器件或电路各个部分的形状和位置**。
    *   通过光刻技术，可以构建例如 **金属层 (metal)**、 **多晶硅层 (polysilicon)**、 **场氧化层 (field oxide)**、 **接触孔 (contact cut)**、 **栅氧化层 (gate oxide)** 以及 **掺杂区 (p+/n+)** 等各种结构。

*   **光刻的多步骤性：**
    *   一个 **完整的器件和电路 (complete device and circuit)** 需要 **许多 (many) 光刻步骤**。
    *   **每个光刻步骤 (each lithography step)**  定义一个 **子组件 (sub-component)** 或一个结构层。

*   **示例：反相器电路 (inverter circuit)**
    *   图中展示了一个反相器电路的例子，说明 **这个反相器电路需要六个光刻步骤** 才能制造完成。  这表明构建一个简单的电路也需要多次光刻操作。
<img width="716" alt="image" src="https://github.com/user-attachments/assets/16043cf4-9942-4230-a464-88c0d3793249" />

**微电子设计通用流程**

**简化IC设计流程图**

1. **定义功能 (Define function)**  -  确定芯片要做什么。

2. **划分设计 (Partition design)** -  把大功能拆分成小模块，方便设计。

3. **高层仿真 (High-level simulation)** -  在较高层次上模拟，验证整体设计思路是否可行。

4. **组装/布局功能模块 (Assemble/layout functional blocks)** -  把各个功能模块拼起来，初步规划它们在芯片上的位置。  同时要考虑 **布局规则 (Layout rules)**， 这些规则限制了设计，例如线间距等等。

5. **低层仿真新模块 (Low-level simulation of new blocks)** -  针对新设计的模块，进行更精细的仿真，看模块功能和性能是否达标。  仿真结果会生成 **器件性能文件 (Device performance files)**，记录模块特性。

6. **检查布局规则冲突 (Check for layout rule violation)** -  检查整体布局是否违反了之前提到的布局规则，确保设计可以实际制造。

7. **生成PG (mask) 文件 (Generate PG (mask) file)** -  PG文件就是光刻掩模版文件，包含了芯片每一层图案的精确信息，是用于 **掩模版制作 (Mask fabrication)** 的最终文件。

**"IC 布局 (IC Layout)"  (也叫 "掩模设计 (mask design)")**

* 是用平面的几何形状来表示集成电路。
* 这些形状对应着金属、氧化物、半导体层等材料的图案。
* 这些层材料构成了集成电路的各种组件。

![image](https://github.com/user-attachments/assets/664a3e73-d06c-4e19-b404-2f9a68b48133)


**光刻曝光系统示意图 (Schematic of Lithographic Exposure System)**。

**主要组成部分 (从上到下):**

1.  **光源 (Optical source):** 提供曝光所需的 **光学能量 (Optical)**，例如紫外光 (UV light) 等。

2.  **光阑 (Aperture):**  控制光束的 **孔径 (aperture)** 大小，可以调节光束的形状和强度。

3.  **快门 (Shutter):**  控制 **曝光时间 (exposure time)** 的开关，决定光线照射到掩模和晶圆上的时长。

4.  **掩模 (Mask):**  也叫 **光掩模 (photomask)**，上面有预先设计好的 **金属图案 (metal shapes)**。  掩模上的图案会 **阻挡 (block) 或透射 (transmit) 光线**，从而形成特定的 **辐射图案 (radiation pattern)**。

5.  **光刻胶晶圆 (Resist wafer):**  **晶圆 (wafer)** 表面涂有 **光刻胶 (resist)**，光刻胶对光线敏感。  **掩模上的金属图案会在晶圆表面创建区域性的辐射图案 (areal radiation pattern)**。

**曝光工具的重要性能指标 (Important measures of performance for exposure tools):**

*   **分辨率 (Resolution):**  **能可靠复制的最小特征尺寸 (the minimum feature that can be reliably reproduced)**。  分辨率越高，就能制造更精细的图案。

*   **套准精度 (Registration):**  **层与层之间的对准精度 (the overlay accuracy from layer to layer)**。  在多层光刻工艺中，确保每层图案精确对齐非常重要。

*   **产能/吞吐量 (Throughput):**  **每小时处理的晶圆数量 (the number of wafer processed in one hour)**。  吞吐量越高，生产效率越高。

**底部文字信息:**

*   **掩模上的金属形状会在晶圆表面创建区域性的辐射图案 (The metal shapes on mask will create an areal radiation pattern on wafer surface)**。 再次强调了掩模的作用，它决定了晶圆上最终的光照图案。

*   **光学光刻有三种不同的方式：接触式、邻近式和投影式 (There are three different ways of optical lithography: contact, proximity and projection)**。  提到了三种不同的光学光刻方法，后续可能会详细讲解。

*   **光刻胶曝光和显影过程中的化学过程 (The chemical processes in photoresist exposure and development)**。  暗示了光刻不仅仅是光学过程，还涉及到光刻胶的化学变化。
![image](https://github.com/user-attachments/assets/cf21a4a3-a63f-4dac-bde1-1147ca432756)

**曝光工具 - 阴影投影 (Exposure Tools - Shadow Printing)**，具体是 **接触式 (Contact printing)** 和 **邻近式光刻 (proximity printing)**。
<img width="600" alt="image" src="https://github.com/user-attachments/assets/94aeef00-ad1a-4869-b633-1132cf6b51a1" />

**核心内容：**

*   **接触式光刻 (Contact printing):**
    *   掩模 **紧贴 (in close contact)** 光刻胶。
    *   **优点:** 分辨率好 (good resolution)，设备简单 (simple equipment setup)。
    *   **缺点:**  掩模易污染和损坏 (photomask contamination and damaging)。

*   **邻近式光刻 (Proximity printing):**
    *   掩模和光刻胶之间有 **间隙 g (gap g)**。
    *   **优点:**  掩模污染和损坏小 (minimum photomask contamination and damaging)，设备简单 (simple equipment setup)。
    *   **缺点:** 分辨率较低 (lower resolution)，分辨率取决于间隙大小。 最小线宽或关键尺寸 (CD) 近似等于根号 g  (CD ≈ √g)。

**总结：**  阴影投影分为接触和邻近两种方式，各有优缺点，主要区别在于掩模是否接触光刻胶以及分辨率的高低。



<img width="787" alt="image" src="https://github.com/user-attachments/assets/9c50efc1-e378-4cdc-afca-907d25bd0213" />


<img width="700" alt="image" src="https://github.com/user-attachments/assets/f1ae3b59-3f77-440b-bdc2-40cc02df0b7b" />

<img width="433" alt="image" src="https://github.com/user-attachments/assets/e1c83975-b065-420b-bf86-d7b547d3c28b" />

<img width="717" alt="image" src="https://github.com/user-attachments/assets/654acfb8-f715-41a1-a92d-e40a7ed28613" />

<img width="470" alt="image" src="https://github.com/user-attachments/assets/2230d122-bcad-4246-991b-830b10bf68aa" />

<img width="453" alt="image" src="https://github.com/user-attachments/assets/c2191108-70f7-4f7b-8ee6-8f5186d1e076" />

<img width="303" alt="image" src="https://github.com/user-attachments/assets/8ffec299-e395-412c-bfaa-9e016b5ac181" />

<img width="694" alt="image" src="https://github.com/user-attachments/assets/1e6bc71a-332a-4d63-b69e-d0587e837d3a" />

<img width="732" alt="image" src="https://github.com/user-attachments/assets/c4a23a8d-7465-4a9f-ba83-fcd39250cdaf" />

<img width="784" alt="image" src="https://github.com/user-attachments/assets/06b7bc60-91d1-4b8d-9694-07fd8355f75b" />

<img width="790" alt="image" src="https://github.com/user-attachments/assets/311fec97-1b63-440c-94d6-d3c238c68784" />

<img width="665" alt="image" src="https://github.com/user-attachments/assets/e16dac0f-a65c-40a5-a072-688fe76e818e" />

<img width="646" alt="image" src="https://github.com/user-attachments/assets/e271b7f2-cd4a-4f5d-affe-6479b27bc999" />

<img width="646" alt="image" src="https://github.com/user-attachments/assets/a832fc21-b5ef-448a-99a9-b9dc85535d96" />

<img width="676" alt="image" src="https://github.com/user-attachments/assets/fbdf97c2-129c-422d-b0f8-d548bd278049" />

<img width="404" alt="image" src="https://github.com/user-attachments/assets/9730c6da-ef24-45c2-84e6-8e17e17de529" />

<img width="801" alt="image" src="https://github.com/user-attachments/assets/5d30ccdf-e506-41e3-ae01-0acb097193b2" />










