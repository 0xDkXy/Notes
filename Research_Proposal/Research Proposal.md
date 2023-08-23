## 3. Project Objectives (Purpose of porposed investigation)

### Origin
The proposed investigation delves into the sphere of computer security, with a specific focus on bolstering the safeguarding of mobile systems, particularly within OpenHarmony OS. The research is driven by several core aims: developing effective techniques to unearth source code vulnerabilities, pioneering innovative methods for detecting malware applications, and devising robust security mechanisms to shield OpenHarmony OS users. By addressing these multifaceted challenges, the study seeks to notably heighten the security posture of OpenHarmony OS while also contributing substantively to the broader domain of mobile system security. By strategically amalgamating techniques such as code analysis and dynamic assessment, the research endeavors to establish a resilient protective framework that ensures secure user interactions and reinforces the operating system's integrity.

This investigation's significance is underscored by its potential to bridge critical security gaps within OpenHarmony OS, a new frontier in mobile operating systems. The aim is to not only enhance security in the immediate context but also to influence the larger landscape of mobile system security, ultimately fostering an environment where innovation and user protection seamlessly coexist.

## 4. Scope and Background of Research: 
(Please identify key issue/problems to be addressed)

### Origin
OpenHarmony, also known as OHOS, stands as an open-source iteration of HarmonyOS, generously contributed by Huawei to the OpenAtom Foundation. This innovative platform marks a new era in mobile operating systems, intended for deployment on smart devices such as Android smartphones and various embedded terminals. With nearly four years of development, OpenHarmony has gained substantial traction, becoming increasingly prevalent not only within smartphones but also across a spectrum of embedded devices.

As its adoption continues to expand, the imperative of fortifying its security becomes even more pronounced. The vulnerabilities that might surface within OpenHarmony's framework carry the potential to inflict harm upon both end users and developers alike. Take, for instance, the looming threat of malware applications seeking to pilfer sensitive user data, including payment credentials. Even more concerning are scenarios where such malicious applications gain control over users' devices, orchestrating attacks on other vulnerable systems. This peril is not to be underestimated.

In light of these escalating security concerns, safeguarding devices, operating systems, and their users takes on paramount importance. Within this context, the primary objectives of this research crystallize. Namely, it aims to chart pathways for unearthing vulnerabilities latent in OpenHarmony's source code, and to develop methodologies for identifying applications that bear the hallmarks of malware. Furthermore, the study will delve into mechanisms and strategies for shielding both the operating system and its users from the potential onslaught of malware attacks.

These research objectives naturally delineate the scope of this endeavor. The investigation encompasses multifaceted elements, including meticulous source code analysis, innovative techniques for malware detection, and an incisive analysis of applications within the OpenHarmony ecosystem. By addressing these crucial dimensions, this research aspires not only to fortify the security of OpenHarmony but also to contribute substantively to the overarching field of mobile operating system security.

### New

#### what can write
the reasons or factors of malware
- permission system exploitation
- lack of awareness and poor practice and skill

## 5. Research Methodology

### Origin

The research methodology for this study encompasses a range of strategic approaches, each meticulously tailored to extract insights and enhance the security of OpenHarmony OS. The following methods delineate the roadmap for investigation:

Static Analysis:

OpenHarmony applications, crafted using JavaScript and the superset ArkTS, often contain pivotal JSON files like app.json5 and module.json5, housing vital configuration information. Static analysis facilitates the comprehensive examination of these files without execution. The analysis of configuration files extracts critical details like package names and permissions, fortifying the understanding of application characteristics. This method also extends to code analysis, focusing on the source code itself. Code analysis delves into elements such as API calls, information flow, taint tracking, native code interactions, clear-text analysis, and opcodes, thereby unveiling intricate nuances in application behavior.

Dynamic Analysis:

Dynamic analysis harnesses the power of execution within a controlled sandbox runtime environment. This approach mandates a fully realized product, an OpenHarmony application complete with multiple HAP packages. By executing the application within this controlled setting, vulnerabilities and potential malware instances can be effectively identified. The potency of dynamic analysis lies in its capacity to scrutinize real-time behaviors during application runtime.

Hybrid Analysis:

Hybrid analysis ingeniously combines the strengths of both static and dynamic paradigms. It begins with decompilation to leverage static attributes such as permissions and intents. Subsequently, the application is executed within an emulator to discern intricate behaviors, culminating in a holistic understanding of application dynamics.

Machine Learning Methods:

Incorporating the prowess of machine learning (ML) and deep learning (DL), this research employs a diverse range of algorithms, including Naive Bayes (NB), Logistic Regression (LR), Decision Trees (DT), Random Forests (RF), Gradient Boosting (GB), Long Short-Term Memory networks (LSTM), Recurrent Neural Networks (RNN), and Multi-Layer Perceptrons (MLP). These techniques take center stage in vulnerability detection, where the generalization of source code into a structured format lays the foundation. By training neural network models on extensive datasets, the study endeavors to pinpoint vulnerabilities embedded within the source code and the nefarious behaviors exhibited by malicious applications.

The fusion of these methodologies represents a cohesive and multifaceted approach to comprehensively address the challenges posed by OpenHarmony OS security concerns. By delving deep into static, dynamic, hybrid, and machine learning realms, this research strives to create a robust and comprehensive framework for enhancing system security.

## 6. Project Significance and Value
### Origin
The surge in mobile device usage is becoming a daily reality in our technological era. Mobile marketplaces are continually flooded with an expanding array of applications to meet the diverse needs of smartphone users. With the ongoing evolution of mobile smartphones and the burgeoning development of Huawei's phone and embedded terminal business, the prominence of OpenHarmony as a versatile operating system continues to rise. Yet, as this wave of innovation sweeps in, it brings along a tide of cyber threats. These challenges underline the critical importance of ensuring the security of OpenHarmony's system. This imperative is magnified in our contemporary digital epoch, wherein the adage "prevention is better than cure" resonates deeply. By delving into comprehensive research on OpenHarmony's security landscape, specifically focusing on robust methods to identify and address vulnerabilities within this operating system, this endeavor is not only a crucial preventive measure but a testament to the ongoing evolution of digital security practices.

The dynamic nature of the cybersecurity landscape accentuates the urgency of proactive security measures. As cyber threats evolve in complexity, addressing system vulnerabilities becomes paramount. OpenHarmony's expanding user base makes this research all the more significant. A secure operating system fosters user trust and confidence, essential factors in driving adoption rates higher. By committing to bolster OpenHarmony's security, Huawei positions itself as a trailblazer in the industry, setting a gold standard for security practices.

Furthermore, this project contributes to technological innovation. The methodologies developed for identifying vulnerabilities in OpenHarmony's system can serve as blueprints for enhancing security practices across the tech spectrum. This ripple effect stands to enrich the entire technology landscape. Additionally, the economic ramifications cannot be ignored. A fortified security ecosystem can entice more developers, thereby expanding the app repertoire, driving user engagement, and potentially resulting in elevated revenue streams.

Collaboration serves as a cornerstone of this project. Engaging experts, researchers, and stakeholders in the cybersecurity domain not only addresses immediate concerns but also cultivates a collective repository of knowledge. This reservoir of insights can serve as a valuable resource for aspiring cybersecurity professionals and scholars.

The significance of this research transcends OpenHarmony alone. The insights gained can be applied to fortify the security of other operating systems, making a broader impact on digital security practices. Furthermore, by addressing emerging regulations and standards for digital security and privacy, this research contributes to ensuring regulatory compliance.

Ultimately, this research empowers OpenHarmony users. A fortified security framework bestows users with confidence in their devices and data, enabling them to harness the full potential of their mobile experience. In essence, this project is more than just about OpenHarmony's security; it's a cornerstone in the edifice of digital resilience and innovation.

## 7. Details of Any External Collaboration
In these circumstances, are there likely to be any complications associated with the publication of your thesis? Give details.

### Origin
In the context of external collaborations pertaining to my research proposal, it is important to address potential complications that might arise in connection with the publication of the thesis. These complexities primarily stem from the unique nature of the research endeavor focusing on the system security of OpenHarmony.

One notable aspect that warrants attention is the absence of readily available developing tools and comprehensive research resources pertaining to the system security of OpenHarmony. As a result, the entirety of the research process will necessitate an independent and self-reliant approach. This implies that a substantial portion of the tools required for the research will need to be conceptualized and developed in-house. The absence of off-the-shelf tools may introduce challenges in terms of time allocation and resource management, as the creation of these tools can potentially extend the research timeline.

Moreover, OpenHarmony stands out as a sprawling and intricate operating system, capable of functioning across diverse devices employing a variety of instruction sets. The complexity inherent in such a multifaceted system presents a formidable challenge, demanding a deep and comprehensive understanding for effective review and analysis. Given the extensive scope of OpenHarmony and its diverse applications, comprehending its intricacies for the purpose of conducting research could prove to be an arduous undertaking.

The sheer scale of OpenHarmony's applicability further accentuates the challenges associated with comprehending and evaluating its security mechanisms. Multiple devices, each utilizing different instruction sets, necessitate a thorough investigation into the potential vulnerabilities across these diverse environments. This intricate landscape calls for an exhaustive examination, which, in turn, may amplify the time and effort required to complete the research objectives.

In light of these challenges, the collaboration landscape becomes crucial. While external collaboration could potentially ease certain burdens by providing access to expertise and resources, the intricate and unique nature of the research topics at hand may limit the extent to which external partnerships can be leveraged. The specialized knowledge required for understanding and securing a diverse operating system like OpenHarmony may not be readily available within external collaborations, necessitating an internal and specialized approach.

To address the potential complications stemming from these circumstances, a meticulously planned and adaptable research strategy will be essential. This strategy should encompass a proactive approach to tool development, rigorous self-education in the intricacies of OpenHarmony, and a systematic plan for managing the complexities of multi-device and multi-instruction-set applications. Ultimately, by acknowledging and embracing these challenges, the research can be conducted with an informed perspective, enabling the generation of valuable insights despite the hurdles presented by the unique nature of the subject matter.