## 3. Project Objectives (Purpose of porposed investigation)

### Origin
The proposed investigation delves into the sphere of computer security, with a specific focus on bolstering the safeguarding of mobile systems, particularly within OpenHarmony OS. The research is driven by several core aims: developing effective techniques to unearth source code vulnerabilities, pioneering innovative methods for detecting malware applications, and devising robust security mechanisms to shield OpenHarmony OS users. By addressing these multifaceted challenges, the study seeks to notably heighten the security posture of OpenHarmony OS while also contributing substantively to the broader domain of mobile system security. By strategically amalgamating techniques such as code analysis and dynamic assessment, the research endeavors to establish a resilient protective framework that ensures secure user interactions and reinforces the operating system's integrity.

This investigation's significance is underscored by its potential to bridge critical security gaps within OpenHarmony OS, a new frontier in mobile operating systems. The aim is to not only enhance security in the immediate context but also to influence the larger landscape of mobile system security, ultimately fostering an environment where innovation and user protection seamlessly coexist.

## Scope and Background of Research: 
(Please identify key issue/problems to be addressed)

### Origin
OpenHarmony, also known as OHOS, stands as an open-source iteration of HarmonyOS, generously contributed by Huawei to the OpenAtom Foundation. This innovative platform marks a new era in mobile operating systems, intended for deployment on smart devices such as Android smartphones and various embedded terminals. With nearly four years of development, OpenHarmony has gained substantial traction, becoming increasingly prevalent not only within smartphones but also across a spectrum of embedded devices.

As its adoption continues to expand, the imperative of fortifying its security becomes even more pronounced. The vulnerabilities that might surface within OpenHarmony's framework carry the potential to inflict harm upon both end users and developers alike. Take, for instance, the looming threat of malware applications seeking to pilfer sensitive user data, including payment credentials. Even more concerning are scenarios where such malicious applications gain control over users' devices, orchestrating attacks on other vulnerable systems. This peril is not to be underestimated.

In light of these escalating security concerns, safeguarding devices, operating systems, and their users takes on paramount importance. Within this context, the primary objectives of this research crystallize. Namely, it aims to chart pathways for unearthing vulnerabilities latent in OpenHarmony's source code, and to develop methodologies for identifying applications that bear the hallmarks of malware. Furthermore, the study will delve into mechanisms and strategies for shielding both the operating system and its users from the potential onslaught of malware attacks.

These research objectives naturally delineate the scope of this endeavor. The investigation encompasses multifaceted elements, including meticulous source code analysis, innovative techniques for malware detection, and an incisive analysis of applications within the OpenHarmony ecosystem. By addressing these crucial dimensions, this research aspires not only to fortify the security of OpenHarmony but also to contribute substantively to the overarching field of mobile operating system security.

## Research Methodology

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