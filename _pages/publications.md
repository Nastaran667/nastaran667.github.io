---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script>
  $(document).ready(function () {
    $(".abstract").hide();
    $(".button").on("click", function () {
        $(this).next(".abstract").slideToggle(400);
    });
});
</script>


<style>
.abstract{text-align:justify; }
.button{ text-align:justify; }
</style>

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}



<ol reversed>
<div id="2">
<li> <b>A Novel QRS Detection Based on the Adaptive Improved Permutation Entropy</b>, <em>Licentiate thesis</em>, 2021 [<a href="/papers/#">pdf</a>] [<a href="https://research.chalmers.se/en/publication/525880">link</a>] [<a href="https://youtu.be/0Mdj-sNxqXU">video</a>]
  <br>Supervisor: Dr. Farah Torkamani Azar, Dr. Hung Cao, Dr. Tadesse Ghirmai
<div class='button' data-content="toggle-text"><a href="#2">abstract</a></div>
<div class='abstract'>
Modular programming is a key concept in software development where the program consists of code modules that are designed and implemented independently. This approach accelerates the development process and enhances scalability of the final product. Modules, however, are often written by third parties, aggravating security concerns such as stealing confidential information, tampering with sensitive data, and executing malicious code.
<p style="margin-top: -0.1%;">
Trigger-Action Platforms (TAPs) are concrete examples of employing modular programming. Any user can develop TAP applications by connecting trigger and action services, and publish them on public repositories. In the presence of malicious application makers, users cannot trust applications written by third parties, which can threaten users’ and platform’s security.</p>
<p style="margin-top: -2.5%;">
We present SandTrap, a novel runtime monitor for JavaScript that can be used to securely integrate third-party applications. SandTrap enforces fine-grained access control policies at the levels of module, API, value, and context. We instantiate SandTrap to IFTTT, Zapier, and Node-RED, three popular JavaScript-driven TAPs, and illustrate how it enforces various policies on a set of benchmarks while incurring a tolerable runtime overhead. We also prove soundness and transparency of the monitoring framework on an essential model of Node-RED.</p>
<p style="margin-top: -2.5%;">
Furthermore, nontransitive policies have been recently introduced as a natural fit for coarse-grained information-flow control where labels are specified at the level of modules. The flow relation does not need to be transitive, resulting in nonstandard noninterference and enforcement mechanism. We develop a lattice encoding to prove that nontransitive policies can be reduced to classical transitive policies. We also devise a lightweight program transformation that leverages standard flow-sensitive information-flow analyses to enforce nontransitive policies more permissively.</p>
</div></li></div>

<div id="1">
<li> <b>Securing Node-RED Applications</b>, <em>Protocols, Strands, and Logic: Festschrift in honor of Joshua Guttman'21</em> [<a href="/papers/joshua21.pdf">pdf</a>]
<br><i>Mohammad M. Ahmadpanah</i>, Musard Balliu, Daniel Hedin, Lars Eric Olsson, and Andrei Sabelfeld
<br><a class='button' data-content="toggle-text" href="#1">abstract</a>
<div class='abstract'>
Trigger-Action Platforms (TAPs) play a vital role in fulfilling the promise of the Internet of Things (IoT) by seamlessly connecting otherwise unconnected devices and services. While enabling novel and exciting applications across a variety of services, security and privacy issues must be taken into consideration because TAPs essentially act as persons-in-the-middle between trigger and action services. The issue is further aggravated since the triggers and actions on TAPs are mostly provided by third parties extending the trust beyond the platform providers.
<p style="margin-top: -0.1%;">
Node-RED, an open-source JavaScript-driven TAP, provides the opportunity for users to effortlessly employ and link nodes via a graphical user interface. Being built upon Node.js, third-party developers can extend the platform's functionality through publishing nodes and their wirings, known as flows.</p>
<p style="margin-top: -2.5%;">
This paper proposes an essential model for Node-RED, suitable to reason about nodes and flows, be they benign, vulnerable, or malicious. We expand on attacks discovered in recent work, ranging from exfiltrating data from unsuspecting users to taking over the entire platform by misusing sensitive APIs within nodes. We present a formalization of a runtime monitoring framework for a core language that soundly and transparently enforces fine-grained allowlist policies at module-, API-, value-, and context-level. We introduce the monitoring framework for Node-RED that isolates nodes while permitting them to communicate via well-de ned API calls complying with the policy specified for each node.</p>
</div></li></div>


</ol>







<!-- 
{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
-->
