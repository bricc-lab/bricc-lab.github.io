---
title: "BRICC@MICS Research"
layout: textlay
excerpt: "BRICC@MICS Research."
sitemap: false
permalink: /research/
---

# Research

In our one-of-a-kind lab, we conduct _joint_ research in the hardware and software
domains of Brain-Inspired Computing and Circuits, ranging from low-level
<span style="color:white">Memristors</span>
to high level algorithms for
<span style="color:white">Spiking Neural Networks</span>, with
<span style="color:white">applications in the Wireless Communication domain and
more!</span>

This particular research setting enables
us not only to theoretically contribute to
<span="color:white">Neuromorphic Computing</span>, but also tightly
couple and evaulate the algorithms on our specialized neuromorphic hardware. This
greatly aids in getting the brain-inspired AI technologies closer to real-world
deployment with applications in a variety of domains. Thank you for taking
interest in our research; take a look below on what, why, and how we do research
in our lab, and if enthusiastically intrigued, feel free to contact
<a href="mailto:yangyi8@vt.edu">Dr. Yang (Cindy) Yi</a>.

### Encoders and ASIC Design

![]({{ site.url }}{{ site.baseurl }}/images/respic/enc1.jpeg){: style="width: 300px; float: right; margin: 0px 10px"}

Like biological neural systems, signals can be transmitted as spikes in neuromorphic
neural networks. Thus, a spike encoder is essential for a neuromorphic computing
system. To better understand the functionality of a neuromorphic network, neural
encoding schemes need to be carefully investigated. Such an encoding scheme refers
to converting the information of input stimuli into a set of spike trains, which
the downstream units can process.

![]({{ site.url }}{{ site.baseurl }}/images/respic/enc2.jpeg){: style="width: 400px; float: left; margin: 0px 10px"}

The research about encoding schemes started a few decades ago. There are two main
kinds of encoding schemes, <span style="color:white">Rate Encoding</span> and
<span style="color:white">Temporal Encoding</span>. Rate encoding is an encoding
scheme that maps the input information to the number of spikes within the sampling
window. Rate encoding is easier to understand and implement than other encoding
schemes. Thus, it is more widely realized in software and hardware implementations
than other encoding schemes. Unfortunately, this encoding scheme has the
disadvantage of low data density. Since rate encoding only uses the number of spikes
to convey information, the temporal patterns of spikes in encoding windows are
ignored. On the other hand, temporal codes tend to transmit information with the
temporal patterns of spikes, thus utilizing both the number of spikes and the firing
time of the spikes. Two different types of temporal encoding are commonly
investigated, the <span style="color:white">Time-to-First-Spike (TTFS)</span>
encoding and the <span style="color:white">Interspike-Interval (ISI)</span> encoding.

![]({{ site.url }}{{ site.baseurl }}/images/respic/enc3.png){: style="width: 500px; float: right; margin: 0px 10px"}

With the progress of large-scale data processing applications, the demand for
higher data processing capacity becomes increasingly intense. Researchers have
found an encoding scheme that combines multiple schemes to increase the data
capacity in biological neural systems, called the
<span style="color:white">Multiplexing Encoding</span> scheme. Besides better
encoding capability, multiplexing encoding has some other advantages as well.
This scheme is more stable and robust with an
internal reference frame than other encoding schemes, especially in the noisy
environments. Our group has designed and analyzed the first ISI temporal encoder
and the multiplexing temporal encoder (to the best of our knowledge). These encoder
designs have achieved both - a high training/inference accuracy and extremely high
power efficiency with reasonable design area.

### Memristors-based Neuromorphic Computing

![]({{ site.url }}{{ site.baseurl }}/images/respic/mem1.png){: style="width: 500px; float: left; margin: 10px 10px"}

The data-intensive nature of AI applications makes them
computationally inefficient to run on traditional computing architectures. Due to
the large number of vector-matrix multiplication operations in the Neural Networks,
a significant amount of power is spent on data movement - to and from the memory.
This is a latent limitation of von-Neumann Architecture, on which a majority of
conventional computing-hardware is based. The latency of this data movement
between the computing/processing unit and the memory also limits the throughput
performance of the system.

A <span style="color:white">Memristor</span> crossbar can solve this issue of
increased energy consumption and latency by carrying out large amounts of
vector-matrix multiplication operations in-memory. As an
<span style="color:white">emerging non-volatile memory (eNVM)</span> technology,
the memristor has gained immense popularity in recent years due to their ability
to emulate spiking neurons and synapses to aid in the making of neuromorphic
hardware. With the use of our <span style="color:white">two-layer fabricated VT
memristor</span>, we aim to develop energy-efficient Neuromorphic Computing
architectures. Our work encompasses <span style="color:white">memristor-based
Spiking Neural Networks</span>, <span style="color:white">spiking Reservoir
Computing</span>, as well as in-memory computing architectures.

### Algorithms for Spiking Neural Networks and Loihi

![]({{ site.url }}{{ site.baseurl }}/images/respic/snn1.png){: style="width: 350px; float: left; margin: 10px 10px"}

One of crucial aspects of information processing in our brain is the generation
and transmission of action potentials, a.k.a. spikes.
<span style="color:white">Spiking Neural Networks (SNNs)</span> are the next
generation Neural Networks which employ spiking neurons to accomplish general
AI tasks. Unlike the Artificial Neural Networks (ANNs), they are inherently
temporal in nature, with few works advocating SNNs to be more robust and
potentially more powerful than ANNs!

![]({{ site.url }}{{ site.baseurl }}/images/respic/snn2.png){: style="width: 350px; float: right; margin: 10px 10px"}

So far, in our attempts to develop brain-like AI, we have been working with the
conventional ANNs for long (since the start of 1940s), which are composed of
highly abstracted out non-spiking neurons. The recent breakthroughs in AI can be
largely attributed to the coupling of effective ANN training techniques and
suitable hardwares e.g. GPUs/TPUs. But this has come at the cost of high energy
consumption while training and inferencing; this is not at all scalable for edge
devices or battery powered critical AI systems. SNNs on the other hand, in
conjunction with specialized neuromorphic hardware e.g.
<span style="color:white">SpiNNaker</span>, <span style="color:white">Loihi</span>,
<span style="color:white">TrueNorth</span>, etc. offer the promise of low-power
and low-latency AI!

In this lab, we actively work in the field of Neuromorphic Computing to develop
<span style="color:white">spiking network algorithms</span> with a focus on their
deployability on specialized neuromorphic hardware, e.g.,
<span style="color:white">Intel’s Loihi</span>. We also collaborate with other
(hardware) teams in this lab to develop novel neuromorphic hardware customized
spiking networks for applications in wireless communication domain, apart from
the general AI tasks.

### Neuromorphic Computing in Communications

![]({{ site.url }}{{ site.baseurl }}/images/respic/comm1.jpg){: style="width: 250px; float: right; margin: 10px 10px 10px"}

Brain-Inspired computing, such as
<span style="color:white">Reservoir Computing</span>, provides a new paradigm of
data-driven algorithm design for communication systems. The rich dynamics behavior
of Reservoir Computing may help build simplified signal detection algorithms using
efficient training techniques.

Future communication systems, such as the
<span style="color:white">5G/6H wireless networks</span>, face many new design
and implementation challenges. For example, traditional model-based algorithms
may not scale well with massive <span style="color:white">MIMO antenna systems</span>
and have model mismatch problems in real-world environments. Furthermore, their
high complexity hinders power efficiency for mobile and IoT applications.

![]({{ site.url }}{{ site.baseurl }}/images/respic/comm2.jpg){: style="width: 250px; float: left; margin: 0px 10px 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/respic/comm3.jpg){: style="width: 250px; float: left; margin: 0px 10px 10px"}

We have adopted <span style="color:white">Echo State Networks (ESN)</span> and
demonstrated their superior performance in a real-time
<span style="color:white">Software-Defined Radio (SDR)</span> testbed. Our
<span style="color:white">ESN-based MIMO-OFDM</span> symbol detection system is
more resilient and power efficient than conventional algorithms widely used in
the current 5G systems. We are also exploring other types of Neuromorphic Computing
techniques for applications in wireless systems.

### Neuromorphic Computing and FPGA

![]({{ site.url }}{{ site.baseurl }}/images/respic/nfpga1.jpg){: style="width: 400px; float: right; margin: 0px 10px"}

Neuromorphic Computing is based on the <span style="color:white">non-von Newman</span>
architecture, which breaks the memory bottleneck of the traditional computing chips
to achieve low-power, low-cost, and low-latency design.
<span style="color:white">FPGA-based Neuromorphic Computing</span> design focuses
on the hardware implementations of neuromorphic computing systems and architectures
on FPGA and the associated optimizations on it.

![]({{ site.url }}{{ site.baseurl }}/images/respic/nfpga2.jpg){: style="width: 250px; float: left; margin: 0px 0px"}

![]({{ site.url }}{{ site.baseurl }}/images/respic/nfpga3.png){: style="width: 275px; float: left; margin: 0px 10px"}

Due to the novel architecture of neuromorphic computing, it has better computation
efficiency on temporal tasks than traditional Neural Networks such as Recurrent
Neural Networks (RNNs). However, neuromorphic computing chips such as Intel's Loihi,
are still not mature enough to implement all kinds of circuits. Many ideas about
the architectural optimizations on the neuromorphic computing systems need to be
verified in time, which is easily doable on FPGAs - a reconfigurable and mature
platform for circuit design.

We have been working on new architectural designs of the typical models of
recurrent networks such as, <span style="color:white">Echo State Network (ESN)</span>,
<span style="color:white">Delayed Feedback Reservoir (DFR)</span>, etc., adapting
them to neuromorphic systems with their designs implemented and verified on the
FPGA platforms.

<!-- **Ultra-stable SI-STM instrument.**  ![]({{ site.url }}{{ site.baseurl }}/images/respic/STMHead.png){: style="width: 250px; float: right; margin: 0px 10px"}

**Magnetic fluctuations and electron spin resonance.**
![]({{ site.url }}{{ site.baseurl }}/images/respic/SpinFluc.png){: style="width: 70%; float: center; margin: 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/respic/SciPost.png){: style="width: 70%; float: center; margin: 0px"}

### ... and more. -->
