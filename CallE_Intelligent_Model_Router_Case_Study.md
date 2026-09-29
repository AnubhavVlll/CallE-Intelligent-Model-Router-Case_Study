# **CallE — Intelligent Model Router**

***Reducing enterprise GenAI operating cost without sacrificing support quality or safety***

**Role:** Hybrid AI Product Manager \+ AI Project Manager

**Company:** CallE 

**Industry:** B2B customer-support SaaS

**Delivery horizon:** 12–16 weeks for MVP / pilot

**Primary KPI:** AI Cost per Resolved Interaction

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

## **Evidence & Disclosure**

This is a **simulated case study**. It is designed to demonstrate product judgment, AI decision-making, technical understanding, and project delivery not to claim real CallE production outcomes.

| Label | Meaning |
| :---- | :---- |
| **FACT** | Information established in the case-study brief |
| **ASSUMPTION** | A reasonable value used because real information is unavailable |
| **HYPOTHESIS** | A proposition the MVP is designed to test |
| **TARGET** | A desired future outcome |
| **SIMULATED / ILLUSTRATIVE** | Example analysis used to demonstrate decision-making |

No simulated customers, research, benchmarks, financial results, production deployments, or AI performance are presented as real evidence.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

# 

# 

# **1\. The Hook**

CallE processes approximately **100,000 AI support interactions per month**, with every request currently routed to the highest-capability model selected as its baseline.

The product question is not:

***“Which LLM is best?”***

It is:

***Can CallE reduce the cost of resolving customer issues while maintaining an agreed quality threshold and keeping risky decisions under human control?***

That reframes the problem from model selection into **business-value optimisation under quality, cost, latency, reliability, privacy, and safety constraints**.

# **2\. Executive Summary**

CallE is a B2B customer-support SaaS platform whose AI capability helps customers resolve support issues and helps human support agents handle escalated cases.

The current workflow uses a premium LLM for every interaction.

This creates a potential economic inefficiency because support requests vary substantially in:

* Complexity  
* Token volume  
* Risk  
* Context requirements  
* Need for reasoning  
* Need for human intervention

A simple FAQ should not automatically consume the same model capability as a complex troubleshooting request. Conversely, a high-risk security or payment issue should not be routed to a cheaper model merely because it is cheaper.

### **Proposed solution**

Build a **hybrid intelligent model router** that combines:

1. Deterministic safety and business rules  
2. AI-assisted intent and complexity classification  
3. A model-selection policy  
4. Response validation  
5. Premium-model fallback  
6. Human escalation

### **Primary objective**

***Reduce AI Cost per Resolved Interaction while maintaining quality at or above the premium-model baseline.***

### **Secondary objectives**

* Increase automated resolution  
* Reduce unnecessary premium-model usage  
* Reduce human support workload  
* Improve escalation quality  
* Establish repeatable model governance

The project is intentionally structured as a **controlled hypothesis-validation exercise**. 

# **3\. Business Context**

## **3.1 Company**

**CallE** is a B2B customer-support SaaS company.

Its product provides AI-assisted customer support across business-specific support workflows.

## **3.2 Primary users**

### **Customers**

Customers interact with CallE to:

* Ask support questions  
* Troubleshoot problems  
* Obtain product information  
* Resolve routine issues  
* Escalate unresolved issues

### **Support agents**

Agents handle cases that AI cannot safely or reliably resolve.

They need:

* A concise issue summary  
* Customer intent  
* Relevant context  
* Suggested category  
* Suggested response  
* Reason for escalation  
* Confidence / risk signal

## **3.3 Business problem**

**FACT:** The scenario assumes 100,000 AI interactions per month and a premium-model workflow for every request.

**PRODUCT PROBLEM:** CallE may be paying premium-model economics for requests that do not require premium-model capability.

But simply moving requests to cheaper models could reduce quality or increase human workload.

Therefore the actual problem is:

***How can CallE optimise model economics while protecting customer experience, support operations, and safety?***

# **4\. Why the Problem Matters**

If CallE does nothing:

* AI infrastructure/API spend may grow with usage.  
* Premium-model usage remains high.  
* Simple requests may consume unnecessary capability.  
* The company has limited ability to optimise model economics by request type.  
* Human workload may remain unnecessarily high when AI fails without useful escalation context.

If CallE over-optimises:

* Quality may fall.  
* More requests may require human intervention.  
* High-risk cases could be mishandled.  
* Customer trust could decline.  
* Apparent AI savings could become operational costs.

The strategic objective is therefore:

***Optimise the economics of successful, safe resolution,not merely the price of an LLM call.***

# **5\. Root Cause**

The visible problem is:

***AI costs are high.***

The deeper product problem is:

***The current workflow does not differentiate model capability requirements across heterogeneous support requests.***

A support platform receives:

* Simple FAQs  
* Summaries  
* Classification  
* Standard troubleshooting  
* Complex reasoning  
* Long-context questions  
* Ambiguous requests  
* High-risk requests

These have different capability and risk profiles.

# 

# 

# 

# 

# **6\. AI Opportunity Map**

| Problem | Traditional solution | AI opportunity | Human role | Recommendation |
| :---- | :---- | :---- | :---- | :---- |
| **Simple FAQ** | Static rules/search | Lightweight model where appropriate | Exception handling | Automate |
| **Classification** | Rules / ML classifier | AI-assisted classification | Review edge cases | Hybrid |
| **Summarisation** | Template/rules | LLM summarisation | Validate escalation context | Automate with controls |
| **Troubleshooting** | Decision trees | Model \+ authorised context | Escalate failures | Hybrid |
| **Complex reasoning** | Rules become difficult | Higher-capability model | Review when uncertain | Premium \+ controls |
| **High-risk request** | Deterministic policy | AI assists interpretation | Human decision | Human-controlled |
| **Account-specific action** | Workflow automation | AI can interpret intent | Authorised agent performs action | Human-controlled |
| **Uncertain response** | Retry/rules | Confidence \+ validation | Human review | Escalate |

### **Product conclusion**

AI is useful for **interpreting variable natural-language requests**, but deterministic rules and humans remain essential for safety-critical decisions.

# **7\. Product Vision**

***Make every CallE AI interaction economically efficient without compromising the quality or safety of customer support.***

## **Mission**

***Route each support request to the least expensive eligible model capable of safely resolving that request, with validation, fallback, and human escalation when necessary.***

## 

## **Product goal**

Validate whether intelligent routing can improve unit economics while preserving the quality of the existing premium-model workflow.

## **Value proposition**

For CallE:

***Use premium AI capability where it creates value, not by default.***

For customers:

***Receive fast, reliable support with human intervention when automation is inappropriate.***

For support agents:

***Receive better-prepared escalations instead of starting each case from scratch.***

# **8\. Product Strategy**

## **Principle 1 — Quality before optimisation**

Cost reduction is only valuable if support quality remains acceptable.

## **Principle 2 — Risk overrides cost**

A high-risk request should never be routed to a cheaper model simply because it is cheaper.

## **Principle 3 — Capability-based routing**

The decision should be:

***“What is the least expensive eligible capability for this request?”***

not:

***“What is the cheapest model?”***

## **Principle 4 — Human escalation is a product outcome**

Some requests should deliberately leave the automated path.

## **Principle 5 — Evidence before scale**

The routing strategy must be validated experimentally before broad rollout.

# **9\. Current-State Journey**

![][image1]

### **Current pain points**

* Every request receives premium-model capability.  
* Model cost is not differentiated by request requirements.  
* Failed AI interactions create human workload.  
* Agents may need to reconstruct the conversation.  
* There is limited routing intelligence between request characteristics and model selection.

# **10\. Future-State Journey**

![][image2]  
 

# **11\. Routing Logic**

The router evaluates four major dimensions:

### **1\. Risk**

Is automation permitted?

### **2\. Complexity**

What level of reasoning is required?

### **3\. Context requirement**

Does the request require authorised support context?

### **4\. Confidence**

Is the system sufficiently confident to proceed?

Then the policy engine considers:

* Quality eligibility  
* Cost  
* Latency  
* Reliability  
* Privacy/security  
* Model availability

# **12\. Routing Policy**

Incoming request  
       |  
       v  
Risk assessment  
       |  
       \+---- High risk \------------------\> Human escalation  
       |  
       v  
Intent / complexity / context  
       |  
       v  
Eligible-model policy  
       |  
       \+---- Simple / low risk \----------\> Lower-cost eligible model  
       |  
       \+---- Moderate \-------------------\> Mid-tier eligible model  
       |  
       \+---- Complex \--------------------\> Premium model  
       |  
       v  
Response validation  
       |  
       \+---- Pass \-----------------------\> Customer  
       |  
       \+---- Fail \-----------------------\> Premium fallback  
                                             |  
                                             \+-- Safe resolution \--\> Customer  
                                             |  
                                             \+-- Still unresolved \--\> Human

# **13\. High-Risk Guardrails**

The following cases should bypass normal cost optimisation or require human review:

* Refund/payment disputes  
* Account/security issues  
* Highly frustrated customers  
* Sensitive personal information  
* Requests requiring account-specific actions  
* Medical/safety-related queries  
* AI uncertainty / low confidence  
* Other business-specific risks

### **Guardrail principle**

***A request can be cheap to process but expensive to get wrong.***

Therefore risk is a **hard eligibility constraint**, not simply another weighted score.

# **14\. Human-in-the-Loop Design**

## **AI completely resolves the issue**

Customer → AI → validated answer → resolved

## **AI cannot safely resolve**

Customer  
   ↓  
AI attempt  
   ↓  
Validation failure / uncertainty / risk  
   ↓  
Ticket creation  
   ↓  
Human agent  
   ↓  
Investigation  
   ↓  
Agent response  
   ↓  
Resolution

The human path is not treated as an AI failure alone.

The product should optimise the **handoff quality**.

# **15\. Agent Context Pack**

When AI escalates a case, the agent should receive:

| Field | Purpose |
| :---- | :---- |
| **Issue summary** | Understand the case quickly |
| **Customer intent** | Understand what the customer wants |
| **Suggested category** | Speed up triage |
| **Relevant knowledge/context** | Reduce investigation effort |
| **Suggested response** | Accelerate drafting |
| **Actions attempted** | Avoid duplicate work |
| **Reason for escalation** | Explain why automation stopped |
| **Confidence/risk signal** | Support agent judgment |

### **Product principle**

***When AI cannot resolve the issue, it should still reduce the human's work.***

# **16\. RAG Decision**

RAG is deliberately **not a new MVP build**.

CallE can use existing authorised support-context capabilities where available.

Potential knowledge sources include:

* FAQs  
* Product documentation  
* Previous support tickets  
* Internal policies  
* Troubleshooting guides

### **MVP boundary**

***Use existing authorised retrieval/context capabilities; do not build a new RAG/vector infrastructure layer during MVP.***

### **Phase 2**

Evaluate a dedicated retrieval architecture if pilot evidence shows it is necessary.

This protects the MVP from unnecessary technical scope.

# **17\. Product Requirements**

## **Functional Requirements**

### **FR-001 — Risk Classification**

The system shall identify requests that require mandatory human review.

**Acceptance criteria**

* **Given** a request matching a mandatory high-risk condition    
* **When** the routing process begins    
* **Then** the request is prevented from entering the normal low-cost automated path.

### **FR-002 — Complexity Classification**

The system shall classify the approximate complexity/capability requirement of an interaction.

### **FR-003 — Context Assessment**

The system shall determine whether authorised support context is required for reliable resolution.

### **FR-004 — Model Selection**

The system shall select an eligible model according to the routing policy.

### **FR-005 — Response Validation**

The system shall validate generated responses before automated delivery.

Validation should consider:

* Correctness  
* Relevance  
* Completeness  
* Safety  
* Groundedness where applicable  
* Confidence  
* Resolution suitability

### **FR-006 — Premium Fallback**

If a lower-cost model fails validation but the request remains safe for automation, the system shall retry using the premium baseline.

### **FR-007 — Human Escalation**

The system shall create/escalate a support case when:

* The request is high risk.  
* Confidence is insufficient.  
* Validation fails critically.  
* Premium fallback cannot safely resolve the issue.

### **FR-008 — Agent Context Pack**

Escalated cases shall contain structured AI-generated context.

### **FR-009 — Automated Resolution**

An interaction shall be counted as AI-resolved only when the issue is completely resolved without human involvement.

### **FR-010 — Audit Trail**

The system shall retain the routing and outcome path for evaluation and governance.

# **18\. Non-Functional Requirements**

### **NFR-001 — Security**

* Authentication  
* Authorisation  
* PII controls  
* Secure API communication  
* Vendor data-use review  
* Access logging

### **NFR-002 — Performance**

Routing and validation must stay within an acceptable support latency budget.

### **NFR-003 — Availability**

A model/API failure must not become a single point of failure for support.

### **NFR-004 — Scalability**

The architecture must support increasing interaction volume without requiring a proportional increase in premium-model usage.

### **NFR-005 — Auditability**

Routing decisions and escalation reasons should be traceable.

# **19\. AI Requirements**

### **AIR-001**

Model routing must respect mandatory safety constraints.

### **AIR-002**

Model eligibility must be evaluated by support-task category, not only overall average performance.

### **AIR-003**

Lower-cost models must have a safe fallback path.

### **AIR-004**

AI-generated customer responses must be validated before automated delivery.

### **AIR-005**

Model/policy changes must be evaluated against the established benchmark before controlled deployment.

# **20\. User Stories**

***As a customer, I want CallE to resolve routine support issues quickly so that I don't need to wait for a human agent.***

***As a support agent, I want escalated cases to contain a clear issue summary and context so that I can investigate faster.***

***As a product manager, I want to measure cost per resolved interaction so that I can determine whether routing creates real economic value.***

***As a support leader, I want risky requests escalated to humans so that automation does not compromise customer safety or trust.***

# **21\. Prioritisation**

For this MVP, **MoSCoW** is appropriate because the immediate delivery problem is scope control within a 12–16 week window.

| Capability | Priority | Rationale |
| :---- | :---- | :---- |
| **Risk classification** | Must | Safety gate |
| **Complexity classification** | Must | Core routing input |
| **Model routing** | Must | Core hypothesis |
| **Response validation** | Must | Quality gate |
| **Premium fallback** | Must | Recovery path |
| **Human escalation** | Must | Safety/resolution |
| **Agent context pack** | Must | Reduce handoff cost |
| **Automated resolution** | Must | Primary outcome |
| **Historical-ticket context** | Must | Support workflow |
| **Customer-facing AI** | Must | Core user experience |
| **Agent assist** | Must | Handoff efficiency |
| **New RAG infrastructure** | Won't — MVP | Scope control |
| **Executive dashboard** | Won't — MVP | Measurement can exist without UI |
| **Fine-tuning** | Won't — MVP | Not required to test hypothesis |
| **Voice support** | Won't — MVP | Unrelated to core hypothesis |
| **Autonomous financial actions** | Won't — MVP | High risk |

# **22\. Roadmap**

## 

## **Discovery**

Define the business problem, baseline, benchmark and guardrails.

## **Prototype**

Prove routing and fallback mechanics.

## **MVP**

Build the end-to-end controlled workflow.

## **Pilot**

Compare dynamic routing against the premium baseline.

## **Production**

Deploy only after pilot gates pass.

## **Scale**

Expand model coverage, categories, retrieval and channels based on evidence.

# **23\. Technology Decision**

## **Options considered**

| Option | Strength | Weakness | Decision |
| :---- | :---- | :---- | :---- |
| **Premium model for all requests** | Strong quality baseline | High cost | Baseline |
| **Cheapest model for all** | Low model cost | Quality/safety risk | Reject |
| **Rules only** | Explainable | Limited language flexibility | Insufficient |
| **LLM chooses everything** | Flexible | Governance/opacity risk | Reject |
| **Single-model optimisation** | Simple | Provider dependency | Limited |
| **Hybrid routing** | Flexible \+ controllable | More orchestration | **Recommend** |

### **Recommended architecture**

***Hybrid routing with deterministic safety controls, AI-assisted classification, policy-based model selection, validation, premium fallback and human escalation.***

# **24\. Architecture**

![][image3]

## **Component responsibilities**

### **Risk engine**

Determines whether automated handling is permitted.

### **Complexity / intent analysis**

Interprets the natural-language request.

### **Context assessment**

Determines whether authorised support information is required.

### **Routing policy engine**

Applies model eligibility rules and optimisation criteria.

### **Model layer**

Generates the response.

### **Validator**

Checks output quality and safety.

### **Fallback**

Provides a recovery path.

### **Human escalation**

Provides safe resolution when automation is inappropriate.

### **Audit/evaluation data**

Supports measurement, troubleshooting and governance.

# **25\. Product Manager vs Technical Ownership**

A critical boundary in this project:

| Area | Product Manager | Engineering | ML/AI | Project Manager |
| :---- | :---- | :---- | :---- | :---- |
| **Business problem** | **Own** | Consult | Consult | Consult |
| **PRD** | **Own** | Input | Input | Input |
| **Routing policy** | **Define** | Implement | Advise | Track delivery |
| **Quality threshold** | **Define** | Support | **Measure/evaluate** | Track |
| **Model implementation** | Decide requirements | **Build** | **Optimise/evaluate** | Coordinate |
| **Architecture** | Contribute | **Own technical design** | Contribute | Coordinate |
| **AI benchmark** | Define decision need | Support | **Execute** | Track |
| **Security controls** | Define requirements | Implement | Support | Coordinate |
| **Delivery plan** | Define priorities | Estimate | Estimate | **Own** |
| **Risks** | Product risks | Technical risks | AI risks | **Own project RAID** |
| **Pilot decision** | **Recommend** | Provide evidence | Provide evidence | Coordinate |

The PM is not claiming to have personally built every technical component.

The role is to:

***Identify the problem → define the product → translate requirements → work with technical teams → make informed AI decisions → manage delivery → manage risks → measure outcomes.***

# **26\. Model Evaluation Framework**

## **Evaluation dimensions**

| Dimension | Weight |
| :---- | :---- |
| **Answer quality** | 30% |
| **Cost** | 25% |
| **Latency** | 15% |
| **Reliability** | 10% |
| **Context capability** | 10% |
| **Privacy/security** | 10% |
| **Total** | **100%** |

### **Important decision rule**

The weights are **CallE product decisions for this hypothetical case**, not universal industry standards.

A model that fails a mandatory safety/security requirement cannot compensate through a higher weighted score.

# **27\. Benchmark Design**

### **Benchmark size**

**ASSUMPTION:** 180 curated support scenarios.

| Category | Cases |
| :---- | :---- |
| **Simple FAQ** | 20 |
| **Standard support** | 20 |
| **Summarisation / classification** | 20 |
| **Troubleshooting** | 20 |
| **Complex reasoning** | 20 |
| **Long-context** | 20 |
| **Ambiguous requests** | 20 |
| **High-risk** | 20 |
| **Adversarial / prompt injection** | 20 |
| **Total** | **180** |

### **Benchmark disclosure**

***SIMULATED / CURATED BENCHMARK DESIGN***

The benchmark is not claimed to represent CallE's actual customer population.

# **28\. AI Evaluation**

## **Model quality**

Evaluate:

* Correctness  
* Precision/recall where applicable  
* Groundedness  
* Relevance  
* Completeness

## **AI safety**

Evaluate:

* Hallucination  
* PII leakage  
* Prompt injection  
* Unsafe outputs  
* Bias where relevant

## **Product performance**

Evaluate:

* Task completion  
* Automated resolution  
* Human escalation  
* Agent time saved  
* Latency

## **Business performance**

Evaluate:

* AI cost  
* AI Cost per Resolved Interaction  
* Productivity  
* ROI

# **29\. Experiment Design**

## **Hypothesis**

***If CallE routes lower-risk and lower-complexity interactions to appropriately capable lower-cost models while reserving premium capability for requests that genuinely require it, then AI Cost per Resolved Interaction can decrease without reducing quality below the premium baseline.***

## **Control**

100% of eligible requests  
        ↓  
Premium baseline

## **Treatment**

Risk-aware dynamic routing  
        ↓  
Eligible model  
        ↓  
Validation  
        ↓  
Fallback / escalation where required

## **Primary success metric**

***AI Cost per Resolved Interaction***

## **Quality threshold**

***Treatment quality ≥ premium baseline***

## **Safety threshold**

***No critical safety threshold breach***

## **Decision rule**

Proceed only if:

7. Economic improvement is meaningful.  
8. Quality remains at or above the agreed baseline.  
9. Mandatory safety controls pass.  
10. Operational impact is acceptable.

# **30\. Economics**

## **Baseline**

The baseline cost model begins with:

***100,000 monthly interactions × premium-model cost per interaction***

But request sizes vary, so a more realistic model needs token-volume assumptions.

### **Illustrative request profiles**

| Profile | Input tokens | Output tokens |
| :---- | :---- | :---- |
| **Short** | 500 | 150 |
| **Medium** | 1,500 | 400 |
| **Long** | 4,000 | 1,000 |

These values are **ASSUMPTIONS**, not CallE measurements.

## **Cost model**

For each interaction:  
Model cost \= input tokens × input price \+ output tokens × output price

At product level:  
AI Cost per Resolved Interaction \= Total variable AI cost ÷ AI-resolved interactions

A complete economic model should also include:

* Routing/classification cost  
* Validation cost  
* Fallback calls  
* Retrieval/context costs where applicable  
* Human operational impact

# **31\. Why Cost per Request Is Not Enough**

Consider two hypothetical strategies:

### **Strategy A**

Very cheap model.

* Low AI cost  
* Poor resolution  
* High escalation

### **Strategy B**

Moderately higher AI cost.

* Higher resolution  
* Lower escalation  
* Better customer outcomes

Strategy A may look better if we only measure:

***Cost per interaction***

But Strategy B may create more business value.

Therefore the primary economic KPI is:

***AI Cost per Resolved Interaction***

# **32\. Illustrative Scenario — Not a Result**

The following is deliberately **SIMULATED / ILLUSTRATIVE**.

| Strategy | Cost | Quality | Interpretation |
| :---- | :---- | :---- | :---- |
| **All premium** | High | Strong | Safe baseline; weak optimisation |
| **Aggressive low-cost routing** | Low | Below threshold | Reject |
| **Balanced routing** | Lower | At/above threshold | Potential candidate |

The product decision is not:

***“Choose the strategy with the lowest cost.”***

It is:

***Choose the strategy that creates acceptable economic improvement while preserving quality and safety.***

# **33\. KPI Framework**

## **North-star economic KPI**

### **AI Cost per Resolved Interaction**

Measures economic efficiency of actual AI resolution.

## **Quality guardrail**

### **Quality score**

Treatment must remain at or above the premium baseline.

## **Safety guardrails**

* Critical safety failure rate  
* PII leakage  
* Unsafe automation  
* Incorrect high-risk routing

## **Supporting metrics**

| Metric | Purpose |
| :---- | :---- |
| **Automated resolution rate** | AI effectiveness |
| **Premium-model usage %** | Routing efficiency |
| **Fallback rate** | Routing quality |
| **Human escalation rate** | Workload transfer |
| **Cost / interaction** | Raw economics |
| **Cost / resolved interaction** | **Primary economic KPI** |
| **Latency** | Customer experience |
| **Quality score** | **Primary guardrail** |
| **Safety failure rate** | **Critical guardrail** |

# **34\. Project Charter**

## **Objective**

Validate whether intelligent model routing can reduce CallE's AI Cost per Resolved Interaction without reducing quality below the premium baseline.

## **Scope**

Design, build and pilot:

* Risk classification  
* Complexity classification  
* Model routing  
* Response validation  
* Premium fallback  
* Human escalation  
* Agent context  
* Automated resolution

## **Out of scope**

* New RAG infrastructure  
* Autonomous refunds  
* Autonomous payment decisions  
* Autonomous account changes  
* Fine-tuning  
* Custom foundation model  
* Voice  
* Global expansion  
* Executive dashboard

## **Deliverables**

* PRD  
* Evaluation benchmark  
* Routing policy  
* Prototype  
* MVP  
* Security assessment  
* UAT  
* Pilot  
* Executive recommendation

## **Timeline**

**12–16 weeks**

## **Constraints**

* Quality cannot fall below the agreed baseline.  
* High-risk automation must remain controlled.  
* Model/API providers create external dependencies.  
* MVP scope must remain limited.

# **35\. Work Breakdown Structure**

## **1\. Discovery**

* Stakeholder alignment  
* Current-state mapping  
* Business objectives  
* Baseline definition  
* Risk taxonomy

## **2\. Requirements**

* PRD  
* User stories  
* Acceptance criteria  
* AI requirements  
* Safety requirements

## **3\. UX / Workflow**

* Customer journey  
* Escalation journey  
* Agent context design  
* Failure states

## **4\. Architecture**

* Routing architecture  
* Policy engine  
* Model integrations  
* Fallback architecture  
* Audit design

## **5\. AI Development**

* Benchmark  
* Risk classification  
* Complexity classification  
* Evaluation  
* Validation

## **6\. Engineering**

* Orchestration  
* APIs  
* Ticket integration  
* Agent workflow  
* Logging

## **7\. Testing**

* Functional QA  
* AI evaluation  
* Safety testing  
* Adversarial testing  
* Integration testing

## **8\. Security**

* PII  
* Vendor review  
* Prompt injection  
* Access control  
* Data retention

## **9\. UAT**

* Support SME testing  
* Acceptance criteria  
* Defect resolution

## **10\. Pilot**

* Control  
* Treatment  
* KPI measurement  
* Failure analysis

## **11\. Launch**

* Readiness review  
* Controlled release  
* Rollback plan

## **12\. Monitoring**

* Quality  
* Cost  
* Resolution  
* Escalation  
* Model review

# **36\. 14-Week Delivery Plan**

| Phase | Weeks | Key deliverable |
| :---- | :---- | :---- |
| **Discovery & baseline** | 1–2 | Product requirements \+ evaluation framework |
| **Model evaluation** | 3–4 | Model evaluation report |
| **Routing prototype** | 5–7 | Working routing prototype |
| **Support workflow** | 8–9 | End-to-end escalation workflow |
| **Testing & UAT** | 10–11 | MVP readiness assessment |
| **Controlled pilot** | 12–14 | Pilot evidence \+ recommendation |
| **Contingency** | 15–16 | Calibration / remediation if required |

The **14-week plan** is the baseline; weeks 15–16 provide contingency for remediation or optimisation.

# **37\. Sprint Plan**

## **Sprint 1 — Baseline**

**Objective:** Establish current state.

**Tasks**

* Current-state mapping  
* KPI definitions  
* Risk taxonomy  
* Benchmark specification

**Definition of Done**

* Baseline workflow documented  
* KPI definitions approved  
* Evaluation scope agreed

## **Sprint 2 — Model Evaluation**

**Objective:** Establish model eligibility.

**Tasks**

* Candidate model selection  
* Benchmark dataset  
* Evaluation rubric  
* Cost model  
* Initial testing

**Definition of Done**

* Benchmark executable  
* Evaluation criteria approved  
* Initial eligibility matrix available

## **Sprint 3 — Routing Prototype**

**Objective:** Prove the core routing mechanism.

**Tasks**

* Risk classification  
* Complexity classification  
* Policy engine  
* Model integration

**Definition of Done**

* Requests can be routed  
* Routing decisions are logged  
* Basic fallback path exists

## **Sprint 4 — Validation & Fallback**

**Objective:** Make routing safe and recoverable.

**Tasks**

* Response validation  
* Quality gates  
* Premium fallback  
* Failure handling

**Definition of Done**

* Invalid responses are blocked  
* Safe failures reach premium fallback  
* Critical failures escalate

## **Sprint 5 — Agent Workflow**

**Objective:** Improve human handoff.

**Tasks**

* Ticket creation  
* Issue summary  
* Intent  
* Suggested response  
* Escalation reason  
* Historical context

**Definition of Done**

* Agent receives a structured escalation package

## **Sprint 6 — Security & UAT**

**Objective:** Validate MVP readiness.

**Tasks**

* PII tests  
* Prompt-injection tests  
* Security review  
* Support SME UAT  
* Defect remediation

**Definition of Done**

* Mandatory safety/security criteria pass  
* UAT acceptance criteria met

## **Sprint 7 — Pilot**

**Objective:** Measure business impact.

**Tasks**

* Control/treatment setup  
* Controlled traffic  
* KPI measurement  
* Failure analysis  
* Executive review

**Definition of Done**

* Pilot evidence collected  
* Scale/iterate/stop recommendation prepared

# **38\. RACI** 

| Activity | PM | Engineering | ML/AI | Data | Security | Support SME |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **Business objective** | A/R | C | C | C | C | C |
| **PRD** | A/R | C | C | C | C | C |
| **Model selection** | A | C | R | C | C | C |
| **Benchmark** | A | C | R | R | C | C |
| **Routing policy** | A/R | C | C | C | C | C |
| **Router implementation** | C | A/R | R | C | C | — |
| **Safety requirements** | A | C | R | C | R | C |
| **Agent workflow** | A | R | C | C | C | R |
| **UAT** | A | R | R | C | C | R |
| **Pilot** | A/R | R | R | R | C | C |
| **Executive recommendation** | A/R | C | C | C | C | C |

**A \= Accountable, R \= Responsible, C \= Consulted**

# **39\. Stakeholder Management** 

| Stakeholder | Power | Interest | Expectations | Decision rights | Communication |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **Executive sponsor** | High | High | Business value and risk | Investment | Biweekly |
| **Product** | High | High | Product outcome | Product policy | Weekly |
| **Support leadership** | High | High | Resolution/workload | Operational acceptance | Weekly |
| **Engineering** | High | High | Clear scope | Technical implementation | 2–3× weekly |
| **ML/AI** | Medium | High | Evaluation clarity | Model evaluation | Weekly |
| **Security** | High | Medium | Safe architecture | Security approval | At gates |
| **Finance** | Medium | Medium | Cost model | Economic validation | At business case/pilot |
| **Support agents** | Medium | High | Useful escalations | UAT feedback | During UAT/pilot |

# **40\. Dependency Register**

| Dependency | Type | Impact | Mitigation |
| :---- | :---- | :---- | :---- |
| **Model APIs** | Vendor | High | Multi-provider fallback |
| **Historical tickets** | Data | High | Confirm access early |
| **Ticketing integration** | Technology | Medium | Prototype early |
| **Security approval** | Security | High | Start during architecture |
| **Support SME availability** | Business | Medium | Reserve UAT capacity |
| **Benchmark dataset** | Data | Medium | Define in discovery |
| **Engineering capacity** | Internal | High | Capacity check before commitment |
| **Provider pricing** | Vendor | Medium | Maintain scenario-based economics |

# **41\. Risk Register** 

| Risk | Probability | Impact | Severity | Mitigation | Owner | Trigger |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **Complex request routed to cheap model** | High | High | Critical | Category thresholds \+ validation \+ premium fallback | PM \+ ML | Quality failure |
| **Quality below baseline** | Medium | High | High | Benchmark gate \+ pilot guardrail | PM \+ ML | Score below threshold |
| **Vendor/API outage** | Medium | High | High | Multi-provider fallback | Engineering | API failure |
| **Savings lower than expected** | Medium | High | High | Pilot before scale | PM | KPI misses target |
| **Hallucination** | Medium | High | High | Validation \+ authorised context | ML | Incorrect response |
| **PII exposure** | Medium | High | High | Redaction \+ security controls | Security | Security test failure |
| **Prompt injection** | Medium | High | High | Adversarial testing \+ guardrails | Security \+ ML | Successful attack |
| **Model drift** | Medium | High | High | Periodic re-evaluation | ML | Performance deterioration |
| **Excessive fallback** | Medium | Medium | Medium | Routing calibration | PM \+ ML | Fallback spike |
| **Latency increase** | Medium | Medium | Medium | Routing latency budget | Engineering | SLA breach |
| **Scope creep** | High | Medium | High | Explicit MVP boundaries | PM/PMO | New feature requests |

# **42\. Governance**

## **Model / routing policy change**

##    **Re-evaluation triggers**

* Provider pricing changes  
* New model release  
* Quality deterioration  
* Increased fallback  
* Changed request distribution  
* Safety incident  
* Provider outage  
* Significant change in context/retrieval behaviour

# **43\. Pilot Design**

## **Control**

***100% of control traffic uses the premium baseline.***

## **Treatment**

***Treatment traffic uses the intelligent routing strategy.***

### **Compare**

* Quality  
* AI cost  
* Cost/resolved interaction  
* Automated resolution  
* Escalation  
* Fallback  
* Latency  
* Safety

### **Pilot decision matrix**

| Outcome | Decision |
| :---- | :---- |
| **Cost improves \+ quality passes \+ safety passes** | Proceed toward controlled rollout |
| **Cost improves \+ quality close to threshold** | Iterate routing |
| **Cost improves \+ quality below threshold** | Reject configuration |
| **Quality passes \+ savings too small** | Reconsider business case |
| **Safety threshold fails** | Stop / remediate |

# **44\. Launch Plan**

## **Alpha**

**Objective:** Technical validation.

**Users:** Internal engineering/AI teams.

**Exit:** Routing, validation and safety paths work.

## **Beta**

**Objective:** Workflow validation.

**Users:** Selected support agents.

**Exit:** UAT passes.

## **Pilot**

**Objective:** Business validation.

**Users:** Controlled customer traffic.

**Exit:** Economic, quality and safety gates pass.

## **Production**

**Objective:** Controlled production deployment.

**Exit:** Stable operating metrics and incident controls.

## **Scale**

**Objective:** Expand model coverage and routing categories.

**Exit:** Continued evidence of economic and customer value.

# **45\. Change Management**

## **Change Request 1 — Add a new RAG system**

### **Original requirement**

Use existing authorised support-context capabilities; no new RAG infrastructure in MVP.

### **Requested change**

Add a vector database and new retrieval pipeline.

### **Impact**

* Engineering scope  
* Security review  
* Evaluation work  
* Additional latency  
* New operational dependency

### **Recommendation**

**Reject for MVP.**

Evaluate dedicated RAG in Phase 2 after validating whether retrieval is a material source of failure.

## **Change Request 2 — Automate payment disputes**

### **Original requirement**

High-risk financial issues require human control.

### **Requested change**

Allow AI to resolve low-value payment disputes autonomously.

### **Impact**

* Financial risk  
* Customer trust  
* Compliance/security considerations  
* New validation requirements

### **Recommendation**

**Reject for MVP.**

Human review remains the control point.

## **Change Request 3 — Add another model provider**

### **Original requirement**

Evaluate a defined candidate model set.

### **Requested change**

Add another provider to the benchmark.

### **Impact**

* Additional benchmark effort  
* Security/vendor review  
* Integration work

### **Recommendation**

**Conditional acceptance** only if the model has a credible capability/cost advantage and can be evaluated without threatening the pilot timeline.

# **46\. Post-Launch Measurement**

## **AI performance monitoring**

* Model quality  
* Hallucination  
* PII leakage  
* Prompt injection  
* Safety incidents  
* Category-level failures  
* Model drift

## **Product analytics**

* Automated resolution  
* Escalation  
* Fallback  
* Agent workload  
* Customer support outcomes

## **Business metrics**

* AI spend  
* Cost/interaction  
* Cost/resolved interaction  
* Productivity

## **Incident management**

Critical incidents should trigger:

11. Automated protection/fallback where available  
12. Incident classification  
13. Technical investigation  
14. Product impact assessment  
15. Corrective action  
16. Model/policy re-evaluation

# **47\. Expected Outcome**

There is intentionally **no fabricated numerical result**.

The expected outcome of the MVP is **decision-quality evidence** answering:

17. Can lower-cost models handle meaningful categories of CallE support traffic?  
18. Can routing reduce premium-model utilisation?  
19. Can this happen without falling below the quality baseline?  
20. Do safety guardrails work?  
21. Does the resulting economics justify the added orchestration complexity?

The project succeeds if it produces enough evidence to make a confident **scale / iterate / stop** decision.

# **48\. Executive Decision Memo**

## **Recommendation**

***Approve a controlled 12–16 week MVP/pilot to test intelligent model routing rather than approving a full production rollout upfront.***

### **Why this solution?**

CallE's issue is not simply expensive LLMs.

It is the mismatch between:

***Request requirements ↔ model capability ↔ model cost.***

A hybrid router addresses that mismatch while preserving human control over risky cases.

### **Why now?**

The scenario assumes 100,000 monthly AI interactions, making AI unit economics strategically relevant.

### **Why AI?**

Support requests are expressed in natural language and vary in intent, complexity and context requirements.

### **Why this architecture?**

It combines:

* Deterministic safety  
* AI classification  
* Policy-based routing  
* Multiple model options  
* Validation  
* Premium fallback  
* Human oversight

### **Why this MVP?**

It tests the central hypothesis without building unnecessary infrastructure.

### **What are we NOT doing?**

* New RAG infrastructure  
* Autonomous financial actions  
* Fine-tuning  
* Voice  
* Global expansion  
* Executive dashboard

### **Biggest risk**

***Routing a complex or high-risk request to an insufficiently capable model.***

### **Biggest assumption**

***CallE's interaction population contains enough lower-complexity, lower-risk requests for routing to create meaningful economic improvement.***

### **What should leadership approve?**

***A controlled experiment—not a guaranteed cost-saving programme.***

# **49\. Retrospective & Critical Thinking**

## **Biggest uncertainty**

The actual distribution of CallE requests by:

* Complexity  
* Token volume  
* Risk  
* Context requirement  
* Resolution outcome

Without this distribution, projected savings remain uncertain.

## **Biggest product risk**

A routing policy could optimise average cost while creating unacceptable failures in important support categories.

## **Biggest technical trade-off**

More sophisticated routing can improve optimisation but introduces:

* More latency  
* More orchestration  
* More failure modes  
* More governance overhead

The router must therefore earn its complexity through measurable economic value.

## **Most important assumption**

There are enough interactions that can be safely resolved by lower-cost eligible models to justify the added routing complexity.

## **What I would validate first with real users**

I would validate:

22. Whether customers perceive quality differences across model paths.  
23. Which support categories agents consider unsafe to automate.  
24. Whether AI-generated escalation summaries actually save agent time.  
25. Which failure types cause the most rework.  
26. Whether customers prefer immediate escalation over low-confidence automated answers.

## **Data required before further investment**

* Actual interaction distribution  
* Actual token consumption  
* Current premium-model spend  
* Baseline quality  
* Automated resolution rate  
* Escalation rate  
* Agent handling time  
* Existing retrieval/context architecture  
* Security constraints  
* Negotiated model pricing

# **50\. What I Would Do Differently**

If this moved from portfolio simulation to a real product, I would **not begin by building the router**.

I would first obtain a representative sample of real support interactions and establish:

***What percentage of requests actually require premium capability?***

Then I would segment those requests by complexity, risk, token volume and resolution outcome.

That data would determine whether routing is worth pursuing.

I would also run the initial experiment offline before changing customer-facing behaviour.

The sequence would be:

Real interaction sample  
        ↓  
Baseline evaluation  
        ↓  
Offline routing simulation  
        ↓  
Failure analysis  
        ↓  
Controlled pilot  
        ↓  
Production decision

This reduces the risk of discovering after implementation that the available optimisation opportunity is too small.

# **51\. Key Product Decisions**

| Decision | Rationale |
| :---- | :---- |
| **Optimise cost/resolved interaction** | Avoid false savings |
| **Premium model remains baseline** | Preserve quality reference |
| **Hybrid routing** | Combine AI flexibility with deterministic control |
| **Risk as a hard gate** | Protect high-risk workflows |
| **Category-specific evaluation** | Prevent averages from hiding failures |
| **Premium fallback** | Recover safe failures |
| **Human escalation** | Preserve human control |
| **Existing context capability** | Avoid unnecessary RAG build |
| **No new RAG in MVP** | Protect timeline |
| **No dashboard in MVP** | Prioritise product validation |
| **Pilot before production** | Evidence before scale |
| **Multi-vendor evaluation** | Reduce provider dependency |

# **52\. Portfolio Artifacts**

This case study can be presented with the following supporting visuals:

27. Executive problem statement  
28. Current-state journey  
29. Future-state journey  
30. AI opportunity map  
31. Model evaluation matrix  
32. Routing decision tree  
33. Architecture diagram  
34. PRD / MVP scope  
35. Prioritisation matrix  
36. 14–16 week delivery plan  
37. WBS  
38. RACI  
39. Stakeholder map  
40. RAID / risk register  
41. Pilot experiment design  
42. KPI scorecard  
43. Governance flow  
44. Executive decision memo

# **53\. Final Thesis**

The strongest way to describe this project is:

***I did not approach the problem as “build an AI router.” I approached it as an enterprise product economics problem: determine whether CallE can use different levels of AI capability for different support requests while maintaining the quality and safety customers expect.***

***I defined the product strategy, decision criteria, quality thresholds, routing policy, guardrails, MVP scope and experiment design; worked across engineering, ML/AI, security and support stakeholders; and structured a 12–16 week pilot to determine whether the economics justified scaling.***

The core lesson is:

***Optimisation is not minimising AI cost. It is maximising business value under quality, risk, operational and cost constraints.***

# 

### **Remaining evidence gap**

The case intentionally does **not** claim:

* Real CallE customer research  
* Real CallE production metrics  
* Real CallE model spend  
* Real CallE benchmark results  
* Real CallE savings  
* Real CallE ROI

Those would require real organisational data.

That limitation is a feature of the portfolio: it demonstrates that the PM can identify **what is known, what is assumed, and what must be validated** rather than manufacturing evidence.

[image1]: <data:image/png;base64,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>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAVwAAAOxCAYAAAC5Ux9ZAABkvUlEQVR4Xuzda5AVVb7nfd/NRDxPxMyr580TMa/G9sWZOGF0TJwxtD0ytjr26NPTeppWjrb2QW2PjgdpW23RRmhvtBdE8YYINLZ4Q0WwQVGEEuUqoNBeaVFBVBS5VHG/FKyH/2LWMmtV7arcuXNl/jP39xOxYu+d+1J/1sr1Y1XWzr2PMUd0dnb2alqEdWmpLaxJc12aa9MgrElLXSKsS0ttYU3UNTCp5ZjkDa1FaqxLaK2NupqntTatdYkq1KWpNqnFB67b0NXVldykgus4bbVprUto29kcrX2mtS7BWDZPa5/1CFwAQDwELgAUhMAFgIIQuABQEAIXAApC4AJAQQhcACgIgQsABSFwAaAgBC4AFITABYCCELgAUBACFwAKQuACQEEIXAAoCIELAAUhcAGgIAQuABSEwAWAghC4AFAQAhcACkLgAkBBCFwAKAiBCwAFIXABoCAELgAUhMAFgIIQuABQEAIXAApC4AJAQQhcACgIgQsABSFwAaAgBC4AFMQHbldXl2+dnZ3Jx5TK1SNNrmviatLYZ8l+04KxbJ7WsRTJPtNEa59JTTZwXWHJpkVYl5bawpo016W5Ng3CmrTUJcK6tNQW1kRdA5NaCNyMwpo016W5Ng3CmrTUJcK6tNQW1kRdA5NafOC6ZbjGX6lcx2n69SWsSUufhTW52xqENWmpK6xJy1gKrWMZ9pmmusI+00Jq6vFHM00DmqRtZ3O01iW07WyO1j7TWpdgLJuntc94lwIAFITABYCCELgAUBACFy2bOnW6GTduAi1lQ/sicNEyCdwf/OAkWsqG9kXgomUSuN99tzXcjMBrr75hA3ffvn22of0QuGgZgZuOC1ytb1lCfAQuWkbgpkPggsBFywjcdAhcELhoGYGbDoELAhctI3DTIXBB4KJlBG46BC4IXLQsRuB2d3ebJ6e9YC668Crz0ANTwrt7WbJ4hXnl5QXhZlUIXBC4aFmMwJ065Rlz4glnm4ULl9rLgUye9JS59Q/3hptVIXBB4KJlMQL3tFMHmyVLVvrbXV07zf79B+z1iY9Os5eyAv700/Vm06bN5rZbxpmrh400G9ZvtPeNuWO8vX75ZdfZ28cde5INZbl8bOI0+/or3n7X/PD4083atevM119/ax935hnnmzc6FtvreSNwQeCiZbECd+nS/gP3kqHXmKefetFeT65wDxw4YLZs2WavS6CKs35yoVm+7B37uqvffd+umh8/UveQ86+wq+gF8xfZx706t8NexkDggsBFy2IE7ojf3W6uGT7KXl+z+gOzZ89es+6Tz82HH6y1gSsBfPDgQbNz5y4z6bEnzUuzXjU/PftiH8qzZs41hw4dMkN/NdzelvvCwJ332kIbxGL79qMB6II3BgIXBC5aFiNwv/7qGxuSEozuGK4cDjj3Z0PNxAlP2BWs3Jb27bffmb1HAvmKy6+3hxWEPEfuW7duvb0tz3t7+bv2kIEE7iknn2P/MHfjiDH2sXJYQcQ6nCAIXBC4aFmMwK0jAhcELlpG4KZD4ILARcsI3HQIXBC4aBmBmw6BCwIXLSNw0yFwQeCiZXUIXHm7WWwELghctKyIwJW3cj304J/s27ncGWTXXjPadHXusO/Fle3ymQvubWDvvfeRvZQz0MSom+82F180zHz00Sf29vTpL9nnyDZ5z6+8P/fn51569IdFQuCCwEXLighcORvsnrsfMatW/dV+oM0dt99vT9+VIJUzxt5/72Pz4PgpPmiXLV1lL+VsNHHBkCvNnDmv22CVwHbv0X193pv2hIpHJ/zZPzcWAhcELlpWVOA6Epb3jp1gPxNBVqoSvk6jwJWz1uTx0oScLHH9dbf6U38ljGMjcEHgomVFBO6bC5f56ytWrLaHAyQsb7pxjP3wGgnhK6+4wQeu3JYzyNypvfKZCfJ4WeFKGMt1eYwcThByJprcjonABYGLlhURuH3ZvXuPv75jx0576QJXPmtBTt1N6uzs8tcPHz7c6/7YCFwQuGhZWYHbF/fhNRoRuCBw0TJNgasZgQsCFy0jcNMhcEHgomUEbjoELghctIzATYfARY/A1bojuLq01aa1LlFkXQRuOlkDt9nHF4X9v3k2cJMdp63QsC4ttYU1aa4rdm0EbjpZAjccx7TPiy2siboGJrX4wO3q6upxqYWrR1ttyQHVVleyz4rY6SRw5eQDWv8tS+AWPZZpVWn/10Lq6hG4rmkrMjmw0jQIa9LSZ2FN7nZM06fPMtOmzTCPP/6ceeyxpxq2Bx+cYh54YLJtcl1a+Ji82i9+8S/mP/7H/7fX9r5aWJNcDx+TZ2smCIoey7TC/V9TXWGfaSE1+WO4rjhtRWqtS2itray69u/f3+tnJ9sXX3zRo4X359luuOEGc8wxx/Ta3qgVWZtraWR5TlGqUJem2qQW3qWA3Ejg7tu3T0X7/e9/bwM33K6pof0QuKil0aNH28AFNGGPRC0RuNCIPRK1ROBCI/ZI1BKBC43YI1FLBC40Yo9ELRG40Ig9ErVE4EIj9kjUEoELjdgjUUsELjRij0QtEbjQiD0StTJo0CAbtGEDNGBPRK10dHT0ClsJYUADAhe15MJWDi0AWhC4qCUOJUAj9kjUFqtbaEPgorbkeC6gCYGLlsl3mv3xj+NpKRvaF4GLlkng/t3f/XdaiiZfIon2ReCiZXxNejruW3v37t1rG9oPgYuWEbjpZPmadNQLgYuWEbjpELggcNEyAjcdAhcELlpG4KZD4ILARcsI3HQIXBC4aBmBmw6BCwIXLUsbuLfdMs62d1b91d6eM3ueOeXkc4JHGbNz5y6zb9/+cLNad9x+f7ipTwQuCFy0LG3gnnnG+WbGC3PMcceeZD79dH14tyeBu3fvvnCzWvLvSYPABYGLlqUN3IsuvMpennbqYDP/9bfMrJlz7fUN6zeaJYtXmHXr1pvu7m4buNu2ddrHHzx40D//s882mFVHVsfj759kLhhypX2ehJ17noT5++99bD7+eJ19/Iq33zVr1nxo1q5dZ77++lv7WPk5r8970z4+eXvhwqX29uRJT9nLxyZOs7VJLXJ706bNdkUuTjzhbPPKywvs9v1HVuJy+d57H5m9e/o/mYHABYGLlqUNXAkmWeVKkMoKds3qD2yobd263dz8+7vMS7NetY+TkLt62Egz9FfDezx///4DZsH8ReaB8ZP98354/On+eRKe48Y+at7oWGxvP36kLglSafI8eaz8HAlzkbwtjznrJxea5cvesa+9+t33bbB+8P5aW7fcf+eYB+3zJPCFbN9zJGRZ4SItAhctSxu4yRXurl27feD+be2n5vDhw+bbb7+zQWcPKRwJMgnMrs4d/vlDzr/CzP7LPHP/fY/ZMJTnyWrWPW/JkpXm0KFDNjRlZTzvtYWmq2unfe727Z32sfJz5Lny+ORtCdSfnn1xr8DdcuTf5QJ148av7eWD46fYSxe4chx69+499mf3h8AFgYuWpQ3ciy8aZi9l5SrhKb/uy4p32dJVNrykya/6EsaympUwvGToNT7Ipj87y//aL6Eoz5NVqnvepMeetNdlm3CHDSQ45bCCe+yI391u70vefnPhMnPuz4aat5e/a2uSwHV/0Hty2gz7GnLIQjz0QM/AlUMSct0dymiEwAWBi5alDdx2R+CCwEXLCNx0CFz0CFytO4KrS1ttWusSRdZF4KaTNXCbfXxR2P+b5wO3q6vLN02FunqkyXVNXE0a+yzZb7ERuOlkCdyix7IZyf1fE619JjXZwHUdl7zUIgxcLbW5mjTWleyzInY6AjedrIFb5FimVaX9X4segRs2LcK6tNQW1qS5rti1EbjpZAnccBzTPi+2sCbqGpjU4g8paC5SY11Ca21F10XgppNH4GpShbo01Sa19PqjmbbjMcJ1nLbatNYlitzZCNx0sgSuaPbxRWH/bx5vC0PLJHAlSGjpmtYwQHwELlr22mtvmL/85TUzc+bLZvr0WSraL395qfkP/+H/6bVdQyNw2xeBi9zs37/fh0nZ7YYbbjDHHHNMr+2aGtoPgYvcHDhwwIauhjZy5EgbuOF2TQ3th8BFLY0ePdoGLqAJeyRqicCFRuyRqCUCFxqxR6KWCFxoxB6JWiJwoRF7JGqJwIVG7JGoJQIXGrFHopYIXGjEHolaInChEXskakVCtq8GaMCeiFoZNGhQr7AlcKEFeyJqxx1OcK2joyN8CFAKAhe15MJWwhfQgsBFLfFHM2jEHonaYnULbQhcACgIgYvaevC+KeEmoFQELmpJvqzxgfGT7eXSpe+EdwOlIHBRO7KylbAVv7zwKhu6gAYELmrFrWxDhC40IHBRC7KqHShU5f7Fi1eGm4HCELiohUYr2yQOL6BsBC4qr9kQZaWLshC4qLTkH8jSYqWLshC4qKw0hxH6w0oXRSNwUUlZVrYhVrooGoGLyml1ZRsidFEUAheVksfKNiQrXQ4toAgELioj75VtEocXUAQCF5UQY2UbYqWL2HzgdnV1+dbZ2Zl8TKlcPdLkuiauJo19luw3LbKOZRFh62hb6WodS5Hc/zXR2mdSkw1cV1iyaRHWpaW2sCbNdWmubSBpTtnNm6aVbthfafqsCGFN1DUwqYXAzSisSXNdmmvrT5Er25CWlW7YXwP1WVHCmqhrYFKLD1y3DNf467HrOE2/voQ1aemzsCZ3W4Owpv7qKmNlG9Kw0tU6luE4aqor7DMtpKYefzTTNKBJ2nY2R2tdQtvO5qTpszJXtiENK90qj2VZtPYZ71KAKhpWtiENK13UA4ELNTStbEOELvJA4EIFjSvbEB92g1YRuCid5pVtiJUuWkHgolRVCltHwx/SUE0ELkpThcMIjbDSRRYELkpRxZVtiJUumkXgonBVXtmGWOmiGQQuClWHlW2I0EVaBC4KU6eVbYi3jCENAheFqOPKNsRKFwMhcFGIuq5sQ6x00R8CF1HV+TBCI6x00QiBi6gkbOt+KKEvrHTRFwIXUbTjyjbEShchAhdRtOvKNsRKF0kELnLFyrY3VrpwCFzkipVt3/hPCILARS5Y2Q6MwwsgcJELVrYD48NuQOCiZYRIc1jpti8CFy0p8pTdV15eYD78YG242ezduy/c1KdZM+ea7u5D4Wbz5Zdfh5uiYqXbvghcZBbzMMIzT880V105wl5fteqvwb09LVy4NNzUlOOO/T78Zv9lnhl1891m5pFwTm6PgZVu+yFw0bQi/kAmgfvzcy818+a9aR55+HG7bcj5V9hVrlyOG/uomTjhCXPnmAdt4D464c/mg/fXmhUrVvd4nR8ef7p5bvpfzK5du81ppw622yRIlyxeYV4/8trd3d329kVHVp1XDxvpn3f5ZdeZs35yob8dC28Zay8ELpomYStBEZME7oknnG2uv+5WM/RXw+22yy75rQ3cM8843656n39utr0vucJd9NZyf13cdss4f90FroTwzb+/y2zb1mlvS+DK60j4OsOvHmn27Nnrb8eyfPk70f/zgh4ELjKJfey2r0MKLnD/tvZTc+7Phvrjsf0FrqyAHRe4H3+8zhw+fNgG+up337eB+/jU6f7+rs4ddlUcmwSttM7OTtPV1WUOHjwYPgQ1Q+Ais5jHcJ99ZpYP3Hf+T+DKr/kSuMuWrrIhecrJ55hhV91k3ly4zD8vDNy77nzIX5eVsZAVrjx/xO9u94cUJIBlNX3o0CHzzTebzQ3X3+afF4Nb2c6fv9gGrgtd1BuBi5bcf8/EaKHbiDsGK6vTn559cXi3esmVrWsHDhwIH4YaInDRsqKPQcrbu24cMcauQuVQQJX0tbKVhvZA4CIXMQ8v1EVfK1vCtr0QuMiFHFooeqVbJY1WthxKaC8ELnLFSrc3F7asbEHgIlesdHtiZYskAhdRsNJtHLZoXz0CV+sOoXVn1VqXKLuudl/pNgrbLCvbsseyEfb/5tnATXactkLDurTUFtakua4ya2vHlW6jsM0iHMesr5O3sCbqGpjU4gNXznJJXmrh6tFWW3JAtdWV7LOyd7p2W+k2CtssK1uhaSyTqrT/ayF19Qhc17QVmRxYLac/hjVp6bOwJne7bO0QunmHrdA4liLc/zXVFfaZFlKTP4ab3EE0Fam1LqG1No11lXEKcJFihK3QOJZOFerSVJvUwrsUUJi6Hl6IFbaoHwIXharjSpewRVoELgpXl5UuK1s0i8BFKeqw0pWwlUbYIi0CF6Wp6kqXlS2yInBRuiqFbqOwBdIgcFG6qhxeaBS2rGyRFoELFbQfXiBskQcCF2poXukStsgDgQtVtK10WdkiTwQu1NG00uWtX8gTgQuVyl7psrJFDAQu1CpzpcvKFjEQuFCt6JUuK1vEROBCvSJXun2tbKUBeSBwUQnX/NtNUUOXlS2KQOCiEkaPHm0DMVbosrJFEQhcVIIErohxeEGC9r77JphjjjmGlS2iInBRCS5wRZ4rXXcoYfbs2T0CF4iBwEUlJANX5LHSTR5GcIHLyhYxEbiohDBwRSsr3fCPZC5wgZjYw1AJfQWuyLLS7esPZK+//jqBi+jYw1AJjQJXSHimFa5sXevo6CBwER17GCqhv8AVaQ4v9LWydX8gI3BRBPYwVMJAgSv6O7zQ16o2+QcyAhdFYA9DJaQJXNHXStcdRuhrZesQuCgCexgqIW3giuRKt6/DCH299YvARRHYw1AJzQSucCvdvg4l9IXARRHYw1AJzQaukJXuQCtbh8BFEdjDUAlZAlcMtLJ1CFwUgT0MlZA1cMXevXvDTb0QuCgCexgqoZXATYPARRHYw1AJBC7qgD0MlUDgog567GFp/rhQhrR/+Cia1rqE9rqarS124CY/D1ebLP1VhKxjWQStdfnA7erq8k1Toa4eaXJdE1eTxj5L9psWrYzloEGDwk25kpokcBnL9JL7vyZa+0xqsoHrOi55qUU4SbXU5mrSWFeyzzTtdK2MZcxf911NP/rRj8ycOXOaqis2rWOZrKfZsYwpWY+m/hI9AjdsWoR1aaktrElzXZprS0MOJ8Q8pJCsR4L9hhtuCB9SmrC/0vZZbGFN1DUwu38lb2gtUmNdQmttrdQlwSahI01+jc+zyQoy2cL7+2pSj/xBK7Zkf0nghnWkba7v8qq5lbGMrQp1aapNaun1RzNtx2OE6zhttWmtS2Td2SQsilhNauuzPOty73jIO3S1ybPP8qa1z+IdGEPlxAzaduN+UwCS2CPgya/EyAfv60Vf2CPgERD5oj8RYo+AR0Dki/5EiD0CHgGRL/oTIfYIeAREvuhPhNgj4BEQ+aI/EWKPgEdA5Iv+RIg9Ah4BkZ28yf6jjz7q0aZOndrj9o4dO8Knoc0ww+ARuNnJ2VYrV67st+3cuTN8GtoMMwwegZsdgYs0mGHwCNzsJHCHX32TueP2cTZcjzv2JLNkyVICFz0ww+ARuNm5wD3+739sFi1a7AP3rjvHmzPPON/cfdcDBC4IXHyPwM3OBe6MGS/Z0HWBO3zYTXZ1e8nQ4QQuCFx8j8DNzgWuDdd/Ge4D99rfjrLbLrvkNwQuCFx8j8DNTgL3N8N/74/XusD91cX/Zq9fd+0oAhcELr5H4GbX37sUFi9ewh/NYDHD4BG42fUXuK4RuGCGwSNwsyNwkQYzDB6Bmy/6EyH2CHgERL7oT4TYI+AREPmiPxFij4BHQOSL/kSIPQIeAZEv+hMh9gh4BES+6E+E2CPgERD5oj8RYo+AR0Dki/5EiD0CHgGRL/oTIfYIeAREvuhPhNgj4BEQ+aI/EWKPgEdA5Iv+RIg9Ah4B0bqOjg7fpD/ddUAww+ARuK1zQRs2QLAnwCMY8jF69GgCF33ye4J8nqdrnZ2dyceUytUjTa5r4mrS2GfJfksrdjC001i6oJXwbUXWsSxCss800dpnUpOdYa6wZNMirEtLbWFNmutKW1vswA1rSltXbGFNedQ1aNCgXPozrCuP2vIQ1kRdA5NaCNyMwpo015W2tjwCoj9hTWnrii2sKa+6Wl3dirCuvGprVVgTdQ1MavGB65bhef1KlZfw11Atv76ENWnps7AmdzuN2IEb1pS2rtjCmrSMpcg6lrGFfaaprrDPtJCaeswwTQOapG1nc7TWJbLsbLEDV8Tosw0bvjRnnfXLltqZZ17gW3hf2S3vuvISYyzzkmX/L0L8GYbKKCJwY5DAvfJfb6ClaD/4wUlh96FA1ZxhiKLKgfv887PDzQjs33/ABq58ezDfIFyOas4wREHg1psLXK2/breDas4wREHg1huBW75qzjBEQeDWG4FbvmrOMERB4NYbgVu+as4wREHg1huBW75qzjBEQeDWG4FbvmrOMERB4Pa26K3l5rZbxtnWl40bvw43NSSPffihqeHmwhC45avmDEMUBG5vH3+8zjw2cZqZ8cKc8C5rzeoPwk0NyWPPPOP8cHNhCNzyVXOGIQoCt29ffPGVv/7zcy81K1euMffc/Yjp6tppg/i99z6y9614+12zZs2HZu3adebrr7/t8fiLLxpmH3vKyeeYD95f61/PGfqr4eGm3BG45avmDEMUBG7fwsAVSxavsJfJFe7jU6ebhQuX2rZg/qIejztv8K8brnDlNY879iT/2rEQuOWr5gxDFARub4cOHTLrP99ouru77e0wcL/6apM97CDmvbbQrnrF9u1HA23JkpX2UgJXHivBunfPXrstiRVue6jmDEMUBG5vcvxWQlKaCANX/PD40+2lhLI87sQTzraHFcSypavspQSuGH//JP/4pL+t/TTclDsCt3zVnGGIgsCtNwK3fNWcYYiCwK03Ard81ZxhiILArTcCt3zVnGGIgsCtNwK3fNWcYYiCwM1O3nd78ODBcHOfZs2ca7q7D4WboyNwy1fNGYYoCNzs5J0Jn/zts3Bzn+TkBwk/eafDKy8vCO+OhsAtXzVnGKJo18B9ctoL5rRTB9uV54oVq+1ZYWPuGG8D6qknZ5hnnp5pT1i44vLr7eOOPmeGGXbVTf52MnCnTnnGnPuzoWbO7Hlm06bNZsj5V/if886qv5qrh430z5G3iMlZa/IzP/roE7v91j/cay8dOYPttlvv67EtCwK3fNWcYYiiXQP3zjEP+utn/eRCe/n8c7PN8KtHmrH3PGLD96EHptjtkx570l7KdmfVkRB1gStnm0nAytlmPz37Ynv/vn377arWcSE9edJTPlzda7zRsdiGtSPb5fHy/t47br/fb8+CwC1fNWcYomjXwJWTERwXdvK5B7ISlWCVQO4vcOWzElzgTpn8tD05Qk6YkCbk2G7yZAcXuPLY0aPusdcPHz5st4+6+W4zccIT/rFyxtpDD/7J1uVOpsiKwC1fNWcYomjXwL38suvsCvKRhx+3hwPkumzbuXOXuXfsBHP3XQ/b0BPJwJWQdWeg3Tduor0uZ5vdOGKMP1zw6afr7XYJVBfs7vMU5BRfOUzhDjF8t3mrD+Okzs6uXM5EI3DLV80ZhijaNXBFV+cOfz3Nuw0kcCVcJZT7snXrdv9OBAnbtOR4biwEbvmqOcMQRTsHbrOSAZ2HXbt2+490jIXALV81ZxiiIHDrjcAtXzVnGKIgcOuNwC1fNWcYoiBw643ALV81ZxiiIHDz0+iPaX0p6oslCdzyVXOGIQoCNz/ffvtduKmhvr52JwYCt3zVnGGIgsBtTL4CR06xlZ8l77GVM8DkfbbypZHJL5aUt4LJl0rKmWZyKc+RxyW/WFLe4yv3yftr5St5Gn2xZN4I3PJVc4YhCgK3MfelkMKdYnv9dbeap596sc+v3XEr3OSpvu41ZEWbPNWXFW77qOYMQxQEbmPymQdyXFbefyufkSDvm3Ur3b4CV04N3r17j/1iSff5DO6LJeXMMvmgHPmMBdHoiyXzRuCWr8cM0zoQri5ttWmtS2Spq4jAjdFnRQSurEIlGN9e/q65Zvgoe13ONpOzyPoKXHfab/JUXzmsIKf6yteuJ0/1bfTFknnLO3BjjGVetNZlZ1iy47QVGtalpbawJs11pa0tduCGNaWtayBFBG4d5Bm44Ti2+np5CWvSUpeQWnzgdnV19bjUwtWjrbbkgGqrK9lnzex0sQM31lgSuOnECtw8x7JVfe3/WkhdPQLXNW1FJgdWmgZhTVr6LKzJ3U6j6MBNW9dACNx0YgRuMjc06Gv/10Jq8jPMFaetSK11Ca21Za0rduBmrWsgBG46eQauiDGWeYi1n7VKaok7w1ApsQM3FgI3nbwDF82r5gxDFASuTuF3nGVF4JavmjMMURC4R7/+RtqhQ0c/PFzeAia35Qsh5Wwy+bJH+bob+QaGDes32rPGrr1mtH2snEkmj3UnMoS35Rt65T28S5eutK+xZcs2u12+Vsd9ieTqd983I2+60z7vyitusF88KW8Zc289awWBW75qzjBEQeAa89KsV+1JCXPmvG5vS1jKd5PJ+2bljLFLhl5jPvtsg71P3mcrgei+dkfeTyuPlW/m7ev2vHlv2ksJbzHzyM8R8r1m8uWR8npyRpr7lt/zBv/aXrLCrY9qzjBE0e6BKyckTHviefuNvS4U5WSGB8ZPNuPGPmrPHJNVqqw431y4zAakfOeZ+7JI+RwFeaz7XrLwtju1V15DuMCVVbT70sm+Atd90WSrCNzyVXOGIYp2D9wdO3baEJVf3+VSTt+VS2lyOMGdbSaBKJ+VsGLFavuZCO4sMflCSLnffU5CeFtWsWLuKx320gWuvJ68hgSzBPkFQ67024V7nVYRuOWr5gxDFO0euEI+vStJPu8g+dm2EsIhWfk64efghrcbkU8Oi43ALV81ZxiiIHDrjcAtXzVnGKIgcOuNwC1fNWcYoiBw643ALV81ZxiiIHDrjcAtXzVnGKIgcOuNwC1fNWcYoiBw643ALV81ZxiiIHDrjcAtXzVnGKKoeuC+8soC2gCNwC1XNWcYoqhq4B44cMB88MHH5r33PjTLl69S0/79v/+/e23T0Ajc8lRzhiGKqgauI5/w5cJEQ5P+DLdpaihetWcYclX1wBUHDx5U06Q/w22aGopX/RmG3NQhcDWhPxFij4BHQOSL/kSIPQIeAZEv+hMh9gh4BES+6E+E2CPgERD5oj8RYo+AR0Dki/5EiD0CHgGRL/oTIfYIeAREvuhPhNgj4BEQ+aI/EWKPgEdA5Iv+RIg9Ah4B0bqOjg7bj2EDBHsCPIIhH4MGDSJw0Sf2BHgEQ35c0I4ePTq8C22MGQaPwM2PW+XKIQbAYYbBI3DzxeoWIWYYPAIXiKvHDNP6SfBaP6Vea10iS11FBG6MPpPvNPvFLy5vqf3TP13qW3hf2S3vuvISYyzzorUuP8O6urp801Soq0eaXNfE1aSxz5L9llbswI01lhK4v7zwKlqKJl8imZfk/q9J1v0/NqnJzjDXcclLLcJJqqU2V5PGupJ91sxOV3Tgpq1rIHxNejrua9J37dplWyuqtP9r0SNww6ZFWJeW2sKaNNeVtrbYgRvWlLaugRC46bjAzaPvw3Fs9fXyEtakpS4htfgZprlIjXUJrbVlravowM0LgZtOnoErYoxlHmLtZ62SWnr90Uzb8RjhOk5bbVrrEll2ttiBK2L0GYGbTqzAzXMs85LXvzFv8WcYKqOIwI2BwE0n78BF86o5wxAFgVtvBG75qjnDEAWBW28EbvmqOcMQRbsF7h23329uu2WcGTf20fCuhpYsXuGv33brfebqYSMT97buh8efbi/nzJ5nTjn5nODe1hC45avmDEMU7Ra4t/7hXnPmGeebCY88bj79dH14d58mT3oq3JQrF7gxELjlq+YMQxTtFrivvfqGuejCq2wQzX/9LbttzB3jzYb1G83ll11nbz/0wBR7edyxJ5lNmzbbFfF7731kHyOP/cPosWbhwqXm0Ql/Nh+8v9asWLHa7Nq127w6t8Ns2bLNvPLyAnPo0CH7Gjt37rKv8/HH68zwq4+ujC8YcmWPn+cCd9bMuea0UwcfCcYue13+Qzh8+LDdJpYve8febgaBW75qzjBE0Y6BKwEoIbd37z5z4MABG5LCBV8ycEVyhSvXXeA6i95abr799juzZ89ee1uC2HGBK+Rny89zt93Pc5drVn9gw1VeL8m93t13PdxjexoEbvmqOcMQRTsGrqxwZ774il2VCllNyop06K+G29vXXXuLvc8F40uzXjWbN2+x4dUocMWom+/24e24wJXnyuEMIcdpkz9P7t+2rdMH7tq168xnn21Ivoy5c8yDmQ49ELjlq+YMQxTtFrjzXltoLr5omOnu7jZDzr/CbjvxhLNt6K1bd/SYrlx3Tew9snKV6/LHsimTn7bB+ebCZf413R/V5DHyWvfc/Yj/1d8FrltVi6VLV/b4eVKP3F6z5kN7fNm9lvv5Qp4rgd4sArd81ZxhiKLdAjcWeYfB6nffNx9+sNYGpRz7FclDClnJOyPOG/xr+59Eswjc8lVzhiEKAjcf+/btN9dfd6s9HLFg/iK/XVa6X321KfHI5snhhmb/WOYQuOWr5gxDFARuvRG45avmDEMUBG69Ebjlq+YMQxQEbr0RuOWr5gxDFARuvRG45avmDEMUBG69Ebjlq+YMQxQEbr0RuOWr5gxDFFUOXAkSWrpG4JanmjMMUVQ1cMWXX24yX3zxlf1gGC3t3/27/6vXNg2NwC1PdWcYclflwBXymQQuTDQ06c9wm6aG4lV7hiFXVQ9cbehPhNgj4BEQ+aI/EWKPgEdA5Iv+RIg9Ah4BkS/6EyH2CHgERL7oT4TYI+AREPmiPxFij4BHQOSL/kSIPQIeAZEv+hMh9gh4BES+6E+E2CPgERD5oj8RYo+AR0C0btCgQbYfw9bR0RE+FG2IGQaPwG2dBGsYtvQrHPYEeARDfpJhO3r06PButClmGDwCNz+ELfriZ1hXV5dvmj66zdUjTa5r4mrS2GfJfksrduC201i6QwutyjqWRUj2mSZa+0xqsnuEKyzZtAjr0lJbWJPmutLWlkdA9CesKW1dsYU15VVXHqvbsK68amtVWBN1DUxqIXAzCmvSXFfa2ghcXXWJsC4ttYU1UdfApBYfuG4ZntevVHkJfw3V8utLWJOWPgtrcrfTiB24YU1p6xqIfKfZT34yJHP7H//jvF4tfExZLawrj9ryEI5jXmPZqr72fy2kph4zrJnJWaRmg6MoWusSWXa22IErYvQZ39qbjvvW3rzEGMu8ZNn/ixB/hqEyigjcGAjcdPia9PJVc4YhCgK33gjc8lVzhiEKArfeCNzyVXOGIQoCt94I3PJVc4YhCgK33gjc8lVzhiEKArfeCNzyVXOGIQoC15iDBw/ay5kz55rNm7cE9xqzY8dOv33fvv1+e3d3t/n662/97bwcOHAg3GR27dpttm7dHm4eEIFbvmrOMETRboE7//W3zG23jLPt1bkddtsnf/vMXp5y8jnmnVV/TTz6qA3rN/rtS5as7LH9h8ef7m/n5b33Pgo3mRkvzDHDrx4Zbh4QgVu+as4wRNFugStOPOHsHrclcPfs2Wt+fu6lZtu2ThvKF180zAbwJ5987reLiY9Os7ffXLisR+DuPfL8004dbJ+XdOOIMeaVlxeYIedfYZYuXWnOG/xrs2XLNvPtt9/Z17962NEQ3blzl7394PgpNnCXLF5hf8594yYeWUkfInArrJozDFG0a+DOm/emOXz4sL0tgXvo0CFz3LEn2SCUS1n9XnH59fZww9q16+x2ISG4Zs2HNhyTgfvwQ1PN+s83mjlzXvc/xz3+p2dfbB9/7s+G2lCeM3ueuWDIlfb5t916n33c41Onm/ff+9iMv3+SDVypYdbMuTao5fEEbnVVc4YhinYN3CR3SMEF7h23328fI+HouMB1hxTkscnAvfyy68xjE6fZJqtlRwJ3wfxFNmBlpXvZJb+1x4rl+UJeQ8jPdCRw5XXd6y16azmBW2HVnGGIol0DV/7gJataIb++y6/tLnBfeH6OGXXz3T2e4wL32mtGm66unTYQv/zyax+cEpjymsK9rmgUuLLilcc98vDj9nGyQpbVtByqcCvcdZ98bg9VbNz4tV3thocr0iBwy1fNGYYo2jFwByIhKe8IWLduvT1MEEq+UyFp9+49R0It/Ye6SHAnybshkiSQJTBbQeCWr5ozDFEQuL3JMdfV775vf5XftGlzeHelELjlq+YMQxQEbr0RuOWr5gxDFARuvRG45avmDEMUBG69Ebjlq+YMQxQEbr0RuOWr5gxDFARuvRG45avmDEMUBG69Ebjlq+YMQxRVDtyJjz5BS9EI3HJVc4YhiqoGrpAA2bZtm/niiy/UNOnPcJuGRuCWp7ozDLmrcuAKORvLhYmGJv0ZbtPUULxqzzDkquqBKyR0tTTpz3CbpobiVX+GITd1CFxN6E+E2CPgERD5oj8RYo+AR0Dki/5EiD0CHgGRL/oTIfYIeAREvuhPhNgj4BEQ+aI/EWKPgEdA5Iv+RIg9Ah4BkS/6EyH2CHgERL7oT4TYI+AREK3r6OjwTfrTXQdEjxmm9Rxrred/a61LZKmriMDV2md51TVo0CDbj2FrRR51xZBXn8WgtS67JyQ7TluhYV1aagtr0lxX2tpaDYaBhDWlrSu2sKZW6xo9enRugRvW1WpteQlroq6BSS0+cLu6unpcauHq0VZbckC11ZXss2Z2ulaCIY12Gstk2EoAZ5V1LGOL0Wd5SNajqb+E1NUjcF3TVmRyYKVpENakpc/CmtztNIoO3LR1xRbWlMdYukMLrco6lrGFfaaprrDPtJCaeh3D1dJxSdp2NkdrXSLLzpZHQAxEa5/FqKuVlW1SlrEsQow+y4vWPos/w1AZRQQu0M6YYfCqGrjynWYnnHAWLWVDeao5wxBFlQP3xhvuoKVo8iWSKE81ZxiiqHLg8jXpA3Nfk75jxw7bULxqzjBEQeDWmwtcrX9QagfVnGGIgsCtNwK3fNWcYYiCwK03Ard81ZxhiILArTcCt3zVnGGIgsCtNwK3fNWcYYiCwK03Ard81ZxhiILArTcCt3zVnGGIgsD93txXOsxxx55knpw2w5xy8jnh3ZVE4JavmjMMURC439vy3VYbuGLihCfs5eWXXWfDt6vz6EkDd4550Jz1kwvNXXc+ZIN54qPTzGmnDjZTpzxj71+xYrW9PeaO8fa2bB95053moQem9Hq+u//cnw01c2bPs7fzRuCWr5ozDC3ZvHmzWbVqVa+2bNmyXttc0yxm4J54wtl+hfvktBfMwoVLzU/Pvtje/uHxp5txYx81+/btN2PvecReF2eecb4NWwlT8fxzR2sbf/8keymvu2fP3h7Pf3zqdDPk/Ct6vH7eCNzyEbhtSAJ35cqVTTXNYgbutdeMNrfdMs5uu3fsBPPYxGlm+vSX7O2PP15nJk96ypw3+Nc2cB8cf3TlKkG7ZMlKu1oVM16YYy/d/S5wk8+fMvlp8/NzL7WvLy0GArd8BG4bInAHtmXLNn9I4YHxk83eIwEpK11Zld504xi7Xe53x3klcC8Zeo29ff11t9r75RCB3JZDEcIdSnCBm3x+d3e3uXHEGLuilp8RA4FbPgK3DUngjhr5Rx+m1107ysyaNbtXyLZz4Dbijt8KCUl3261wd+7c5e8Xu3fv6XE7Kfl8Z+vW7Ue2H+qxLS8EbvkI3DYkgfv222+b+8Y9YpYvf9s8OuFPNlQH/eM5R1ZzE+31J5+cfuRX4n+xxyNnvviX8CVUKTJwG5HgDMNTGwK3fARuG3KHFM7/xa/tr7Ry/bZbx5rJk54wp/94sJk4car56dm/NIN/fqn5y0svs8KtCQK3fARuG3KBO+HIylZWsHL9lj/cbUaPutO2l16aYxYtWmweenCSOf7vf2ymTD76tiitCNx0CNzyEbhtyAWurGT/55lD7HU5tCCrXQnYF198yR5ekNuy0p03b374EqqUFbi7du22l6+8vKDHdjk2m8abC5eFm6IicMtH4LahRu9SWLZsuT22624vemuxv65ZWYH7zNMz7aV7+5fzzTebe9x2lixe0SOcrx42MnFvfARu+QjcNtQocPtrmsUI3HvufsTMmjnXXpcTHrZt67RvC3MnMwgXuPL+WfHJ3z6zh2ie+PNz9nb4HPeWL3lteU33fttnn5llHzP92Vn2trw9TN5iJmep5YnALR+B24YI3IHJyQpy5peQ4Ovq2ml/zvzX3zJ79+6z213gusddecUNZs2aD+2lCJ8jJ1DIqnbD+o1HxmCL+cPosfZxEsSr333fv/9WAnzlyjU2mPNE4JaPwIXHZyn0dNWVI8wjDz9uRt18t5n9l3n2DDM5TXfTpqOHDFzgXnbJb+2lW8m6Qwrhc+RsstGj7rH3CRe4LlhvuP42e+lWzHIIIk8EbvmqOcMQBYHbkxxvleOzy5au8qfldixYbH+ekDPHDhw44AP3oguvsn8we+jBP9nb4XNemvWq/ZwECT7hAle2SUjLSlcQuPVVzRmGKAjc/rl3JfRHTgFOSvMcIcEdG4FbvmrOMERB4NYbgVu+as4wREHg1huBW75qzjBEQeDWG4FbvmrOMERB4NYbgVu+as4wREHg1huBW75qzjBEQeDWG4FbvmrOMERB4NYbgVu+HjNM60C4urTVprUukaWuIgI3Rp9J4MrJBrSBW56BG2Ms86K1Lj/Durq6fNNUqKtHmlzXxNWksc+S/ZZW7MCNNZYSuBIktHSt2f2ikeT+r0nW/T82qcnOMNdxyUstwkmqpTZXk8a6kn3WzE5XdOCmrSutQ4cO9fp3p2lffPGFbxs3brSX4WOyNOnPcFuzzdWTbOFjsrZWJF8nxlhmlawnj39nnnoEbti0COvSUltYk+a60tYWO3DDmtLWlVYegZtnqOURuGFdedUmrRXha7X6enkJa9JSl5Ba/AzTXKTGuoTW2rLWVXTgahKjtjz6M0ZdealCXZpqk1pa3yNQG3kEBL5HfyLEHgGPgMgX/YkQewQ8AiJf9CdC7BHwCIh80Z8IsUfAIyDyRX8ixB4Bj4DIF/2JEHsEPAIiX/QnQuwR8AiIfNGfCLFHwCMgWtfR0eGb9Ke7DghmGDwCt3WDBg2y/Rg2QLAnwCMY8jF69GgCF31iT4BHMOQnGbYSwIBghsEjcPPjDi0ASewR8AiI/Lg/mgFJ7BHwCAggLmYYPAIXiIsZBo/Azc+D902x3x920UX/O7wLbYwZBo/AzY+E7QPjJxO66IEZBo/AbZ1b2SZJ8F5wwRU9tqE9McPgEbitkbCVcO2LC93Dhw+Hd6GNMMPgEbjZ9bWyDcn9rHTbGzMMHoGbTX8r2xAr3fbGDINH4GYz0Mo2xEq3fTHD4BG4zUlzGKERVrrtiRkGj8BtjnvrV1asdNsPMwwegZtOKyvbEG8Zay/MMHgEbjqtrmxD8nocWmgPzDB4BG7/8lzZhji80B6YYfAI3P7lvbJNcqcBs9KtN2YYPAK3sVgr2xAr3XpjhsEjcPvWzIkNrWKlW2/MMHgEbm8xDyP0h5VuPTHD4BG4PRW5sg2x0q0nZhg8Avd7Za1sQ4RuvTDD4BG4R5W5sg1xCnC9+BnW1dXlW2dnZ/IxpXL1SJPrmriaNPZZst/Sih24VRhLLSvbJHd4Yfv27eFdpUru/5pk3f9jk5rsDHOFJZsWYV1aagtr0lxX2tpiB25YU9q6YnO1jP3jw+rC1pG6zjvvMjWhG46jtrHUVpeQWgjcjMKaNNeVtrZ2DlyNK9uQpj+kheOoaSzDpoXU4meY5iI11iW01pa1rqIDV4uiTmrIi5a3jGkcS6F1P5Naesww2aDteIxwHaetNq11iSw7W+zAFdr6TNMfyNLSstLVNpZJWfb/IsSfYaiMIgJXkyocRuiPlpUu0muvGYZ+tVPgVnFlG9Ky0kV67TPDMKB2Cdyqr2xDhG51tMcMQyrtELh1WNmGODmiOuo/w5Ba3QO3bivbJA4vVEO9ZxiaUufArePKNsRKV7/6zjA0ra6B2w5h67DS1a2eMwyZ1DFwY34PmVasdPWq3wxDZnUL3HZa2YZY6epUrxmGltQpcNtxZRtyK13oUZ8ZhpbVJXDbeWUb4vCCLvWYYchFHQKXlW1vnAKsR/VnGHJT9cBlZdsYK10dqj3DkKsqBy4r24Gx0i1fdWcYclfVwGVlmx4r3XJVc4YhiqoGLivb5rDSLU81ZxiiqFrglnUYYePGr81tt4yzbfz9k8K7BzRnzuvmisuvNyN+d7vZsH5jeHchWOmWo1ozDFFVKXDLPoxw2633+etvLlxmfn7upebEE842a1Z/YLdNn/6S3XbxRcPMwYMH7e1TTj7H3nYWLlxqTjt1sL9dNE6OKF51Zhiiq0rglrWyTXKBe+jQIbN06UqzatVfzYYNX5oLhlxptx937ElmyeIV5vV5b5ru7m57e9269fa288PjT7dBXCZOjihWNWYYClGVwBUXXfS/zfLl74SbCyOBO+OFOWbB/EX29lVXjjDPPzfbr1i//fY78+wzs2yobt68xd6+/rpb7W3x1Veb/GuVRfpP/uOaP3+x2bVrFyvdAlRnhiG6KgWukLAoK3SThxTE7L/Ms4cO5LCCBNfHH6+zl3J79bvv29sSunJbzJw512z5bmuP1yia9J8094WLErqIq1ozDFFVLXAl0OTX4bJCN2nvnr1m//4D/rbU1tW5o8dtObTgyOPlcEQZkitbF7bSDhz4vn7EUa0ZhqiqFrhCgqzs47lVE65sCdviVG+GIZoqBq5woathpasZK9vyVXOGIYqqBq6QQwusdPvX18pWGopT3RmG3FU5cAUr3b6xstWj2jMMuap64ApWur2xstWj+jMMualD4ApWut9jZatLPWYYclGXwBWsdL8/lMDKVo/6zDC0rE6BK9p5pdvXYQRWtuWr1wxDS+oWuKIdV7qN/kiG8tVvhiGzOgauaKeTI1jZ6lbPGYZM6hq4QsspwDGxstWvvjMMTatz4Io6H17oa2VL2OrTY4ZpHSStO5DWukSWuooI3DL7TNOH3eSp0co29qGEMsdyIFrrsjMs2XHaCg3r0lJbWJPmutLWFjtww5rS1pW3Oq10y3rrV/jziviZaYQ1aalLSC0EbkZhTZrrSltbuwSuqMNbxvo6jBB7VeuE41jmWCaFNWmpS0gtPnC7urp801SkqydZowZhTVr6LKzJ3U4jduCGNaWtK5Yqr3QbHUYoSjiOZY+l09f+r4XU1OsYrpaOS2o2OIqitS6RZWeLHbhCW59V8S1jZa5sk7SNZVKW/b8I8WcYKqOIwNWoSn9IK3tli9a05wxDn9o1cEUVDi/0tbIlbKulfWcYemnnwNX+lrFGK9syDiUgu/adYeilnQPX0bjSZWVbH8wweASuvpUuK9t6YYbBI3C/p2GlW9ZJDYiHGQaPwP1e2StdVrb1xAyDR+D2VsZKt1HYovqYYfAI3N6KXuk2CltWtvXADINH4DZWROg2ClvUBzMMHoHbWEdHhw3DWKHbKGxZ2dYLMwwegduYBK60GCtdF7b/8A//SNjWHDMMHoHbmAvcGB/r6Fa2P/rRjwjbmmOGwSNwG3OBK/L6Q1p4GMEFLmFbX8wweARuY8nAFXmsdOX5yRMbJHAJ23pjhsEjcBsLA1dkXemGK1vXTjnllPChqBlmGDwCt7G+AtdpJnQbha0YNGhQ8GjUDTMMHoHbWH+Bm/bwQqOwdYcRCNz6Y4bBI3Ab6y9wxUCHFwYKW0Hg1h8zDB6B29hAgSv6W+kOFLaCwK0/Zhg8ArexNIErwpVumpWtQ+DWHzMMHoHbWNrAFcmVbvjWr0ZhKwjc+mOGwSNwG2smcIVb6aZZ2ToEbv0xw+ARuI01G7hCQjdt2AoCt/6YYfAI3MayBK6Q0N21a9eAYSsI3PpjhsEjcBvLGrhCQjcNArf+mGHwCNzGWgnctAjc+mOGwSNwGyNwkQdmGDwCtzECF3lghsEjcBsbPXo0gYuWMcPgEbiNFRGGsQMd5WOGwSNwGyuibyRwZSWN+oq/F6EyigiVMkiQyQpV/n1ZW1EkcMOf3UyT5xPaehW3J0G9IoOlKBK28u+SwHVh1Ewr69f8sI60zf3HAp16jIw7BVGb5OmRmmitS2Spq4iJWnSfpf03FV1XM7LUJf/u2P9Z1K3PimD3xmTHaSs0rEtLbWFNmutKW1vacMoqrCltXa2QVd9AwpqKqCutsK60tclKN+Yf+sKa0tYVW1iTlrqE1OIDt6urq8elFq4ebbUlB1RbXck+a2anix24RY+lrPDSrPK0jqXIOpbyH03M8dTaZ8l6mumvIkhdPQLXNW1FJgdWmgZhTVr6LKzJ3U4j5gQVYU1p68qq2cDVNpYi61gWFbiuvrR1xRaOo7ax9CPiitNWpNa6hNbastYVc4KKrHVllTZwRdG1pZW1rtiBK7LUVYSsfRab1BJ3RFApsSdo0ZoJ3LopInDRPEYEXt0mKIFbr/GsA0YEXt0mKIFbr/GsA0YEXtUnaPhB3wRutcezjhgReFWfoFu2bDErV67st+3fvz98Wi0RuDoxIvCqPkEJ3O8RuDoxIvCqPkElcIdffZNZunSpbcOuGkHgQhVGBF7VJ6gE7nHHnmTuuH2ceeutRfY6gQtNGBF4VZ+gErhj7hhn/nnIv5oli5fYwH3iz8+Yf/ivZ5pnnn7ePPvsCwQuSsWIwKv6BJXA/cOou8yMGS+ZBQvesIE78qY7zPBhN9nV7Z1/vJ/ARakYEXhVn6ASuDePHGPD9fi//7EN3Pvvm2BO//FgM++1+eapJ58jcFEqRgRe1SeoBO6okX+0gfub4b+3gbt8+XLzq4v/zV5fsWIFgYtSMSLwqj5BeVvY9whcnRgReFWfoATu9whcnRgReFWfoN3d3ebgwYO+LVy40LbktnZB4OrEiMCr2wTlsxTqNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq9sEJXDrNZ51wIjAq8sEHTRokP23hK2dELg6MSLw6jJBZVUbhq0EUDshcHViRODVaYKGq9x2Q+DqxIjAq9METa5y2211KwhcnRgReHWcoO0YtoLA1YkRgccErQ8CVydGBF4rE/Tzz7+gpWybNmwKuy93BK5OjAi8ViboD35wEi1lmzZtRth9uSNwdfIj0tXV5VtnZ2fyMaVy9UiT65q4mjT2WbLf0mplgkqQzJ//VrgZgU2bNpsnnnjBHDp0yLaBZB3LIgI3uf9rkrXPYpOa7Ii4jkteahEGrpbaXE0a60r2WTM7XSsTlMBNRwL3sceesmOyb9++8O5eso5l7MCt0v6vRY/ADZsWYV1aagtr0lxX2tpamaAEbjrNBm44jmnHssjAbaau2MKatNQlpBY/IpqL1FiX0Fpb1rpamaAEbjqtBm5asQNXZKmrCFn7LDappceIyAZtx2OE6zhttWmtS2TZ2VqZoARuOs0GrsgylkUGbl32/yLEHRFUSisTlMBNJ0vgDmTlypWp26effho+HQXKPsNQOwRufARue8s+w1A7VQjcHTt2ms2bt4SbU3nvvY/Mhx+sDTebrVu3++sHDx60l838jDRv73II3PaWfYahdmIH7m23jLNt+vSXzIEDB8K7U9mwfqN5Z9Vfw82pnHbqYDPk/CvCzeaG62/z1z/522f2sq/HNbJz564j4bk/3NynGIF7/XV/8IH6h9F39QpZAleP7DMMtRM7cI879iSzd89e89qrb5ifn3upuXHEGPPc9L+Ysfc8YpYsXmG33TduounuPmTve+XlBTb4li5dac4b/Guz58hz5THbth39Y4isWIWE+FNPzjDPPD3TnHnG+WbhwqU2XFclgnn0qHvMVVeOMHNf6TAjb7rT3j/mjvF2ddpX4MrPu/uuh82114y2YSqvfcrJ59jXELJNftZZP7nQB67U96cpz/jX6kuMwJ3wyBSzfPnb5v77Jpi3337bzJk915z4384yQ381zIbsNcNHmh//938yv73mZgK3ZNlnGGqnqMCd8cIcG6QSnhJan322wd43a+Zcu33O7Hn2vp+efbENuXN/NtQGpITj2rXrzLfffmdfb9nSVfbykqHX2ND+4fGnm+FXj7SXVw8baUbdfLf/2UuWrLSvLz9rwfxF9vLEE842y5e902fgSj3Tnnje1ifPW7lyjX3OZZf81t5/79gJ5uOP15kVb79rA1f+E7jowqv8IYlGYgTuihUrjvxH9YgZ9I/n2IA953/9ysx7bf6RvrjJ3pZ/w3PPvWim/ulJArdk2WcYaqeIwJWVojuOKqEq4SckJB+bOM22RW8t9/ddMORKu9J1QScaBe6dYx40Dz0w5civ1WPNpMeetKvkJHdcVn6WhKmsTiXc+wpcd0jhjtvvP7KCfNwG/vPPzbZBLuS5jgSubJfXHUiMwJVQlRXspMcet9eln0ePutM2uT1jxkv2UMPZ//MCArdk2WcYaqeIwJUVrpMMXLlv3Sef2/s3bvw6VeA++8wsG6LNBq6Epxy2kBXuzBdfMTfdOMYfU5ZDG3Kf1COBLqtrOeYst7s6d/g6JGDlcRK20qTux6dOt4/pT6zAPf3Hg82UyU/48JVLObwgl/PmzberYPk3fPLJJ+HTUaDsMwy1EztwByKHDPbvT//HtK6unUdCrzvcnIo8t1kSsEkSrsn/QNKIFbhhW7jwTbNo0WJ7XY7vym25zgq3XNlnGGqn7MBtB0UFbqNG4JYr+wxD7RC48cUI3DVr1vRqixYtMi+//HKv7QRuubLPMNQOgRtfjMDtSxGfpYDmMSLwWpmgBG46BG57Y0TgtTJBCdx0CNz2xojAa2WCErjpELjtjRGB18oEJXDTIXDbGyMCr5UJKoF73i8up6VoBG77YkTg5TFBwy/wK7PNnj3btnC7lkbgth9GBF4eE5TATd8I3PbDiMDLY4IePnxYTevo6LAt3K6lxUTg6sSIwKvbBHWB244IXJ0YEXh1m6AEbr3Gsw4YEXh1m6AEbr3Gsw4YEXh1m6AEbr3Gsw4YEXh1m6AEbr3Gsw4YEXh1m6AEbr3Gsw4YEXh1m6AEbr3Gsw4YEXh1m6AEbr3Gsw4YEXh1m6AEbr3Gsw4YEXh1maASNtIGDRrkr0trJwSuTowIvLpMUAla+bckm2xrJwSuTowIvDpN0DBw2w2BqxMjAq9OEzRc5bYbAlcnRgRe3SaohG67HUpwCFyd/IjI55i6Jp/VqUXy81XluiauJo19luy3tGJPUMayeVnHsojATfaZJln7LDapyY6IKyzZtAjr0lJbWJPmutLWVsQEDZsGYU1a6hJhXWlrix24YU1p64otrElLXUJqIXAzCmvSXFfa2mJOUBHWlLaurJYufcd+15pc9iesKXZdzQjrSlsbgaurLiG1+MB1y3CNv1K5jtP060tYk5Y+C2tyt9OIOUFFWFPaurJwYetaf8KatIylyDqWRQWuqy9tXbGF46htLHuMSDMDWqRmd7aiaK1LZNnZYk5Qp4g+c2G7fPnRla1cNhO62mQZy9iBK+rWZ0WIOyKolNgTtAhh2DqybfHilT221VkRgYvmMSLwqj5BG4Wtk+bwQl0QuDoxIvCqPEEHClvhDi20w0qXwNWJEYFX1QmaJmyT2mGlS+DqxIjAq+oEbSZsRTusdAlcnRgReFWboM2ubEN1XukSuDoxIvCqNkFbDcw6r3QJXJ0YEXhVmaCtrmxDdQxdAlcnRgReVSZoqyvbUB1XugSuTowIPO0TNO+VbVLdQpfA1YkRgad9gua9sg3VKXQJXJ0YEXiaJ2islW2oLqFL4OrEiMDTOkHdoYSi1CF0CVydGBF4Gido7MMIjVQ9dAlcnRgReJomaMw/kDWjrMBvFYGrEyMCT9ME1RJ0VV3pErg6MSLwNExQLSvbUNVCl8DViRGBp2GCalnZhqq20iVwdWJE4JU5QbWubJOqFLoErk6MCLwyJ6jWlW2oKqFL4OrEiMAra4JqX9mGqhC6BK5OjAi8MiZo0Sc15EV76BK4OjEi8IqeoFU5jNCI5tAlcHViROAVOUGr8EeyNFzoakPg6sSIwCtqglZ9ZRvSuNIlcHViROAVMUHrsrINaftPhMDViRGBF3uCagulvGla6RK4OjEi8GJO0LqubENa/lMhcHViRODFmqBVfetXVhpWugSuTowIvBgTtF1WtqGyV7oErk6MCLy8J2i7hq1T5kqXwNWJEYGX5wRt97B1ylrpErg6MSLw8pqghG1PZZwcQeDqxIjAy2OClrWi067owwsErk49RqSzs9M2bVxd2mrTWpfIUlerE5SVbf+y/meUZSyLCNy67f9FsCOS7DhthYZ1aaktrElzXWlra2WCZg2TdtPsSjccx7RjGTtww5rS1hVbWJOWuoTU4gO3q6urx6UWrh5ttSUHVFtdyT5rZqfLOkFZ2Tanmf+cso5lkYGrff/XQurqEbiuaSsyObDSNAhr0tJnYU3udhpZJmiRJzV0d3ebr7/+Ntzcr+3bO83OnbvCzQ0dOnTIvPfeR+Fma+vW7eGmzNKudLOOZVGBm8wNDfra/7WQmvyIuOK0Fam1LqG1tqx1NTtBm13Z3nH7/ea2W8aZcWMfNe+s+mt494A2rN9ofnj86eHmfo0edY+ZOuWZcHNDo26+25x26uBwszX86pHhJmvio9PMkPOvMHff9XB4V7/SrHSzjmXswBVZ6ipC1j6LTWqJOyKolGYmaLNhK1579Q1z0YVX2etDfzXcXkqInnLyOaarc4e9fc3wUTbw5syeZ2+PuWO8OfOM882qIwHtAnf95xv96+zatdts2bLNB+VHH31it987doJ93WuvGd0jcGWFLI+T1xTyuieecLZZs/oDe/u4Y08yV105wl5fsniFfdx94yba2y5wZ7wwx18+OH6KvS7uufsRfz2tWG8ZKyJw0TxGBF7aCZolbIUL3P37D/hVpNz+5pvNNjDFjSPGmL+t/dR88P5af/+6Tz63QesCV37tlzAVr7y8wF5eMORKG8TudSU4ly5daS+TgTvid7fb11+z5kN7+7PPNpgNG760z3fPmzVzrj0MIdc3bdpsV6/CBe65PxtqL+U58lghAd/s6ttJc2ihWQSuTowIvGYnqATFA+Mnh5sbksA9b/CvbVi+OrfDbpNQe2ziNDN9+kv2tqwq5TXlsIN4o2OxvZRVaPKQwocfrPWhKGRlLK8jbc+evX4FHR5S6O4+ZF/fBfPNv7/LPP/c7B5BvXnzFhvI8rPcawoXuPKfg6x63c8QUk8WUsu9d06wv27meRyUwNWJEYHX7AT95S+vbOrXYbfCnfniKz7gzvrJhfbyk799Zi/lEMGBAwfMZZf81t6WQJQVrQThl19+7QNWjL3nEb8yvenGMfaParJ6lcdLQHd2dtmfkwzcea8ttK//6IQ/29uyej148KB9/OHDh33gbvluq/9Ze48EuLj4omH2uoSxPP7pp170r3vnmAf99bQkbKX/kscbpZY8ELg6MSLwskxQCalmQrcv7vit2Ldvf693FXR17exxu5Hdu/f0uN3oeeHryyGORuSdCX3d37Hg6MrbCV9zIMmVrWt79x4N9jwQuDoxIvCyTtALLriiqUMLVSer5uRKu1l9rWwlbOU/r7wQuDoxIvBamaASuq2udNtB7JWtQ+DqxIjAa2WCyuqs3Va6zeprZSstz5WtQ+DqxIjAy2OCstLtW6OVbYywFQSuTowIvDwmKCvdvhW1snUIXJ0YEXh5TlBWukf1dRgh5srWIXB1YkTg5TlBWekeJWEbHkqIHbaCwNWJEYEXY4K260q3rJWtQ+DqxIjAizVB8zg5okoa/YGsSASuTowIvJgTtF0OL/S1si3qMEISgasTIwIv9gSt++GFRivbosNWELg6MSLwYk/QOv8hTcvK1iFwdWJE4BU1Qeu20tW0snUIXJ0YEXhFTdC6rXQ1rWwdAlcnRgRe0RO06ivdvg4jlL2ydQhcnRgReEVP0KqvdMs6qSENAlcnRgReWRO0aqGreWXrELg6MSLwypqg7sSIqoSu5pWtQ+DqxIjAK3OCVuHwQl8rW41hKwhcnRgReGVPUO0r3b5WtkWfspsWgasTIwJPwwTVutKtysrWIXB1YkTgaZmg2la6jU5s0IzA1YkRgadpgmpZ6fZ1GEHzytYhcHViROBpm6Blr3SruLJ1CFydGBF4GidoWSvdqq5sHQJXJ0YEntYJ6la6RanyytYhcHViROBpnqBFHV7oa2VbtbAVBK5OjAg87RP0P/2n/xJ1pSthfu7/d2GvsK3SoQSHwNWJEYGnfYJKfR0dHVFWum5le8MNN1R6ZesQuDr1GBG3o2mTXHFoorUukaWuIiZoK33mAjfvP6RJ2H7xxRe2/eY3v7G1aVrVZumvIgK3lbGMTWtdfkS6urp801Soq0eaXNfE1aSxz5L9llbsCdrqWLrAFXkd03V/IJOw3bhxo7nmmmvMN998Ez6sNFnHsqjAdfVpkrXPYpOa7Ii4jkteahFOUi21uZo01pXss2Z2utgTtNWxTAauaHWl6w4juNWtNHdIQYusYxk7cJP1ZBnLWJL1NNNfRegRuGHTIqxLS21hTZrrSltbzAkqwprS1uWEgSuyvmUs+dYvF7aystUWuGF/pa2tyMBtpq7Ywpq01CWkFj8imovUWJfQWlvWumJOUJG1LqevwBXNHl7o661f27dvt5faAzet2IErstRVhKx9FpvU0uuPZtqOxwjXcdpq01qXyLKzxZ6gopU+axS4Iu33ozU6qcFdHzFiRPiU0mUZyyIDN8tYxpalz4oQd0RQKbEnaKv6C1wx0Eq3r5Vt+NYvCao6KCJw0TxGBJ72CTpQ4IpGK91GK9vw7V8ELmJiROBpn6BpAleEK91GYdsXAhcxMSLwtE/QtIEr3EpXwlYuw7ANV7YOgYuYGBF42idoM4ErJFTTrmwdAhcxMSLwtE/QZgNX7Nq1K9XK1iFwERMjAk/7BM0SuEJCdqCVrUPgIiZGBJ72CZo1cJtB4CImRgSe9glK4KZH4OrEiMDTPkEJ3PQIXJ0YEXjaJyiBmx6BqxMjAk/7BC2ivkGDBoWbKonA1YkRgad9ghax+tTeB2kRuDoxIvC0TFA5bJBssuosqjb5efKzJLCkhbWETSsCVydGBF7ZE9SFRF+tyHCTnxX+/P5aESvvZhG4OjEi8MqcoFqDKw0JaG3HfglcnRgReGVO0DJ/dh6k/iJX4QMhcHViROCVOUGrurp1pO80rXIJXJ0YEXhlTlACN18Erk6MCLwyJyiBmy8CVydGBF6ZE5TAzReBqxMjAq/MCUrg5ovA1YkRgVfmBCVw80Xg6sSIwCtzghK4+SJwdWJE4BU1QQ8ePGi2bNnSo02aNKnH7bTf0FCGsHZpZ511lvntb3/ba7u0MhC4OjEi8IqaoPI9YytXruy3bd++PXyaGmGt/bWPP/44fHohCFydGBF4RU1QAjc+AlcnRgReURNUAvfhhyebpUuX2lAadtWIXkGlOXCvv+4PZsWKFbbOaU8826t2AheNMCLwipqgErjDr77J3HH7OBtKxx17Uq+g0hy4J5/0v8yDDzxmli9/2wz6x3N61U7gohFGBF5RE9QF7j8P+VczauQfbeA+8ednzD/81zPNM08/b47/+x+rDlxZ3f707F/asH3iiWfM72+6w8ye/YoNYQnZe8c+bJ577kUzY8ZLBC56YETgFTVBXeBKIEm4SuCOPBJaw4fdZAPrkqHDVQeu1Pjssy+YC//5Cntd/uOYPOkJM+mxx80bb7xppv7pSXvYQW4TuEhiROAVNUFd4EpYzZkz1wbu/fdNMKf/eLCZ99p8u9LVHrjSpkx+wl7KfxRyeEGuy+r38alP2UtZtX/44Yfh0wtB4OrEiMAraoL29y6FZcuW28sqBG6yLVq02K5u3e2FC9+0ocsKF0mMCLyiJmh/geta1QK3USNwkeRHpKury7fOzs7kY0rl6pEm1zVxNWnss2S/pRV7grqaNm3aZNasWWPee+893958880et4sO3GbGMlmnazNnzjSvvvpqr+0fffRR+PSmZB3LIgI32WeaZO2z2KQmOyKusGTTIqxLS21hTZrrSltbERM0bE6Zn6UQ1pS2v5Kk72J8lkJYV9raYgduWFPaumILa9JSl5BaCNyMwpo015W2tpgTVIQ1JesicPsW1pW2NgJXV11CavGB65bhaX6lKlLyVwNNv76ENWnps7AmdzuNmBNUhDUl69IQuK2MZazAzTqWRQWuqy9tXbGF45hlLGORmnqMSDMDWqRmd7aiaK1LZNnZYk5Qp1GflRm4olFdacUKXJFlLGMHrmi1z2LK0mdFiDsiqJTYE7Q/ZQduq2IGbhZFBC6ax4jAK3OCErj5InB1YkTglTlBCdx8Ebg6MSLwypqgVQ9boS3gtNWDoxgReGVN0DoEbkdHR2n91xcCVydGBF7sCSqhJL92uyY/T1odAtdx/6bkv7OvJv9m6Y9YCFydGBF4MSdooyCKGTplkH+PhF347wyb649YfU7g6sSIwIs1QWOv5qrMrfrzRuDqxIjAizVBY71uXRC47YMRgRdjgmr7Y5ImycMKeR1eCF9PWp2OkVdd6yOM2shjwocI3MbCYMyjn1x/5/mayA+jAS/G5CRw++f+gJbnYYVk6LK61YWZgF4rImmt/pEr/Et83qFSJzH+Q3L9D10YEfQZjq3q61fbVkO8rmL8RyR9zepWn9ZnFmohGbp5TtQ8QxyoOmYBvLzDVsQI8SL8+c/Pm6lTp9NSNqRD4MKL9attFVe3Ex583PzgByeZ777bShugST8hnerNBEQT6xhrrNeNyQUuBib9tH//ftvQPwK3ArZ+s5WWsuWFwE1P+knrV9poQ+Aq99lnG+wOTUvX8kLgpif9ROCmQ+Aq5wIX/duzZ6/tp8OHD9vWKgI3PQI3PQJXOQI3HRe4eX1lN4GbHoGbHoGrHIGbjgvcvCY+gZtenv1edwSucgRuOgRuefLs97ojcJUjcNOpQuB2d3ebJ6e9YC668Crz0ANTwrv79MrLC8JN6uTZ73VH4CpH4KZThcCdOuUZc+IJZ5uFC5fayzRu/cO94SZ18uz3uiNwlSNw06lC4J526mCzZMlKf1uC94IhV9rr76z6q72UFfCnn643mzZttu3qYSPNhvUb7X1j7hhvr19+2XX29nHHnmT+dCTE5fKxidPs6694+13zw+NPN2vXrrOX4swzzjdvdCy212PIs9/rjsBVjsBNpyqBu3Rp/4F7ydBrzNNPvegf41a4Bw4cMFu2bLPXXZCe9ZML7aW87up337er5senTjdDzr/CvvZPz77Y3v/q3A57GUue/V53BK5yRQbu28vftZdvLlwW3KNfFQJ3xO9uN9cMH2Wvr1n9gVn01nJzysnnmLmvdNjA7eraaQ4ePGh27txlJj32pH2chOb+/Qfs9Vkz55pDhw6Zob8a7u8TycCd99pCH8TffvudvVwwf5G9jCXPfq87Ale5IgNXfp0Vj074c3CPflUI3K+/+saGpASjtK7OHTZwb7pxjA1cWcHK4QFpLiyvuPx6e1hByHPkvnXr1tvb5/5sqL2UQwYSuPJa8oe5G0eMsY91K+GYhxNEnv1edwSuckUGrkz8efPeNNdeM9redhNaVk0iecxw6p+etSsrIb++zn/9Lbtd/PzcS83KlWvMPXc/Ym8XoQqBW1d59nvdEbjKFRm44Qo3DNzkr7DC/aVdfoV9/rnZPQJXLFm8wl4WgcAtT579XncErnJlBu55g39tNm/eYi675Lf2dqPAvfn3d5mOBYsJ3DaVZ7/XHYGrXJGB2xc5JjiQNI+JjcAtT579Xnc9Aldrp7m6tNVWRF1lB25VtBq44VhqDdwVK1aHm0rXSr/Hoq0exwZucmfTVmhYl5bawppi1UXgptNK4IbjKE1r4Gok/fTFF1803e8xhOOooSZHavGBKx9pl7zUwtWjrbbkgMasi8BNJ6/AdWMZM3DlbVvPTf+LGXvP0XdxyDHv+8ZNNN3dh8zXX39rhl11kz0hYu+Rf5OcDix/vJwze549xu6OjyffATJxwhP2cfL2MHmckHeJXHzRMP+Hz5i0BW4yMzTU5EhdPQLXNW1FJidDHp91moewplh9RuCmk0fgJscyZuBKaLqzvz54f619n+wN199m7hzzoP3DY2fn9/t4eNbY5ElP2Ut5D6+E88cfr7MnRiQfJyc6yG05a032n9iknzZu3Nh0v8cQjqOGmhwfuMIVp61IrXWJImrTGLhyNtRA5FOuPvxgbbg5mlYCV4RjGTtw3dlfa9Z8aD8HQZqceSaBKyvb5GPd/cIFrnhy2gzzyMOP93qcfBbD7t177Bi4kx9iaqXfYwjHUguphXcpKKcxcD/522fhJsu9fawMrQZuKHbgJs/+klCUoJ3xwhzz+rw3/e1du3b3OmtsyuSnezzPvTVPHifPcR9cI4cX5LasdGPLs9/rjsBVLkbgyvtjk8cNw+N98quqnCYqxxFXrfqrfWxy4rrAle0y4eVzAeRzAmSyyzZZWcml/Bz50BX5lCv3fAlGCRv51XfDhi/9a7aqSoEbks9HcJ+X4G4nf4vYunW7HaeBSF8nHyeBXYQ8+73uCFzlYgSurHySxw2Tx/tkkroTGIQEgfz6+8D4yX6bC1zZLh+o4k6ESK5w5boErwS5O1Ptb2s/tR/M4n5llsDPS5UDt+ry7Pe6I3CVixG4shJNHjdMHu/btq2zR+DKWWRXXTmiRzi6wJXtckqvC1z3Oa3CBa6Eufv1Wf7AI4G7b99+e5vArYc8+73uCFzlYgSu/LEledwwPN4nxxHltrTpz86yl/LHmnFjH7X3y235i7g7ZugCV2qVbfL6Er4SuPIJWXKowh2DlBW0+/WZwK2HPPu97ghc5WIErgiPG4bH++S4oTuOmPyreZJsT75Gfw4fPhxuyhWBW548+73uCFzlYgVu3RC45cmz3+uOwFWOwE2HwC1Pnv1edwSucgRuOlUKXDnOfeUVN9hvdZAvfZSTH+QYt7wdT95mJ6fwynefyZdIymPlj43Drz76rQ/y9errPvncvjtEDunIsXT5OE15vnywTfh8+Ur2b77ZbN+aF0ue/V53BK5yBG46VQvc7zZvtdflSx/7OyXXvWPktVffsJfyNjtH3mYnzxXy2cXyjpO+ni+Pcd+RFkOe/V53BK5yBG46VQtc93kJ8h5l+fJIWe1u395pQ1P+WCnfZSYhKY+VP0y6b++Vr0GSP3guX/aOfXtdGLjh890XSqY5cSKrPPu97ghc5QjcdKoUuKH+zhCTwJX3Lic/5F0Cur93fYTvOJEPupH3WseSZ7/XHYGrHIGbTpUDtz/ukIJmefZ73RG4ykngnnHGL8xpp51nTj11sJr2n//zf+u1TUPLa+JrCdwqIHDTI3ArQo7buZ1aQzvmmGN6bdPUWkXgpkfgpkfgVoQE7o4dO9Q0Cdxwm6bWKgI3PQI3PQK3QuQPJVqaBG64TVNrFYGbHoGbHoGLTCRw64zATY/ATa/eswbRELhwCNz06j1rEA2BC4fATa/eswbRtEvg/t3f/XfaAI3ATa/eswbR1D1wnX379vkwoQ3c0L/2mDXIHYFL66uhf+0xa5C7dglcIE/MGmRC4ALNY9YgEwIXaB6zBpkQuEDzmDXIhMAFmsesQSYELtA8Zg0yIXCB5jFrkAmBCzSPWYNMCFygecwaZELgAs1j1iC1QYMG+SaB6653dHSEDwXQhx6Bq/V8aK3namutS8Sqy4VtsjVDa59prUtor0tzbdr42dLV1eWbpkJdPdLkuiauJo19luy3PMlqNhm2o0ePDh/SEGPZvJhj2apkn2mitc+kJhu4ruOSl1qEk1RLba4mjXUl+yzGTpclbAVj2bzYY5mV1j5L1qOpv0SPwA2bFmFdWmoLa9JcV961SdA2eyhBhDXlXVdWYU1a6hJhXVpqC2uiroFJLX7WaC5SY11Ca23U1TyttWmtS1ShLk21SS29/mgmy15tXMdpq01rXULbzuZo7TOtdQnGsnla+6z53wtRqM8+22C/M4qWrgGaEbjKucDdtGkzbYBG4EI7Alc5F7jo3549e20/af1VEhAErnIEbjoELqqAwFWOwE2HwEUVELjKEbjpELioAgJXOQI3HQIXVUDgKkfgpkPgogoIXOXyCtxZM+eGm0xX5w7T1bUz3FxJBC6qgMBVLkvgLl/2jrntlnG2PfTAFLvtlJPPCR5lzNh7HjEPjj96fyMffrA23BTNksUrwk2pEbioAgJXuSyBK155eYG5YMiV9vo7q/5qrh420l5ftnSVDd/bbr3PB+6C+YvsYzes32jvu/aao58CNuJ3t5vTTh1sfn7upf51hayKzxv86x7btm3rNEN/Ndyc9ZMLzYwX5tht819/y76etI0bvzaXX3advS4razHypjvN1CnPmCuvuME8Oe0Fc+IJZ9ufdc/djyRfOhUCF1VA4CqXR+AKCc5Fby03Pz37Yr9NAlfCTlbE4rhjTzILFy41kx570j9GXidJgk1eQx4bhu6KFavNzJlz7X3ffvudvRTXX3ervZRQldd3NQw5/wp76V5n8qSn7GUWBC6qgMBVLs/AfX3emz7khATuD48/3dz8+7vsbQnIxyZOs82ZM+d1f110d3ebeUdeRx67cuUav332X+bZ1e3zz832QXvH7ffbnytN3Dt2gn3t6dNfsrfDwJ0y+Wl7mQWBiyogcJXLGrhzX+noEbhnnnG+vbz/vsdsIF580TAbgHKMV47TSvDKClUupTnn/myoD1BHQlcOUyR98P7R15DDBO7whby2HCaQwD18+LA9nCCPuenGMfZ+V58L3r1HQlN+lnt+MwhcVAGBq1zWwO3P1q3bzaFDh8LNlhxf3b17T7g5FQliRwJZjsdu395p1q1bb9Z/vtFud8dv80bgogoIXOViBG4R9u3bbx6d8Gdz3bW3+BVtTAQuqoDAVa6qgVs0AhdVQOAqR+CmQ+CiCghc5QjcdAhcVAGBq1zRgSsnKDz80NRwc0OtnB3mJN+qlhWBiyogcJUrOnDXrP7Av4UsjVZOVnAIXLQLAle5PAJX3p716afr7TsH5L2x6z753H6YjbzvdefOXfZMMHkv7iMPP25Py5X3y8r7aoW8V1be0iXvpe3uPmTDUU7HveyS39rvEZPPa3jvvY96/Dw5m0xOYpDXdCdOyL9D3pMrZ7XJ+3/lNOAVb79rNmz40r6m3Df1T8/2eJ1mELioAgJXuVYDd9eu3T1OXJATHpy/rf3UBq4Er7hv3MReK9zRo+6xAepeQ+qRQJawFX2tcOXxjrw1TLw061V7JpoEsPwHIJ/f4MjJFe5DdrIicFEFBK5yrQaunOHlzhyTExPkPbFy0oOsNGXFawN37z57vwTuV19tsuHqQlgeL8+TcJbnSWDLNnc6sATp5s1bjv6w/0MCV1bIEoJyGu/SpSvt6lhWsTNffMWeSXbrH+61P1tOhJBTe+UzHbKcYeYQuKgCAle5VgNXyGcoSIjKavfrr76x110Iy7b9+w/Y6xK4Yvz9k/z98uu+PF4OKcjhBln9yplq7n53Om6SBK6sYmW7BOqOHTvtdflkMrmUwxvyOnL97eXv2sMW8phmjh2HCFxUAYGrXB6BW7TkIYWiELioAgJXuSoGrjtEUSQCF1VA4CpXxcAtA4GLKiBwlSNw0yFwUQUErnIEbjoELqqAwFWOwE2HwEUVELjKEbjpELioAgJXOQI3HQIXVUDgKucCl5auEbjQzAduV1eXb5p2WFePNLmuiaupiD6T02pdPwzUNm7caNsXX3xhW3h/WS1Zk1wP78+zNUueU9RYNiNZk6a6RLLPNNHaZ1KTDdxwZ9VUZFiXltrCmmLXlTZwXaCFLXxcGS2sKWZdzQif2+zzYwrr0lJbWBN1DUxqIXAzCmvSXJfm2jQIa9JSlwjr0lJbWBN1DUxq8YFblUMKWn59CWvS0mdhTe62BmFNWuoKa9IylkLrWIZ9pqmusM+0kJp6/NFM04AmadvZHK11CW07m6O1z7TWJRjL5mntM96lAAAFIXABoCAELgAUhMAFgIIQuABQEAIXAApC4AJAQQhcACgIgQsABSFwAaAgBC4AFITABYCCELgAUBACFwAKQuACQEEIXAAoCIELAAUhcAGgIAQuABSEwAWAghC4AFAQAhcACkLgAkBBCFwAKAiBCwAFIXABoCAELgAUhMAFgIIQuABQEAIXwP/fTh2jMBDDUBC9/23tGwQtOMi/WbYRU8wDE9IN0iIN8eBK0hAPriQN8eBK0hAPriQNuQ7uWut5NKeL1kbtKvQuWhu1q9C7yG00z8Htg6OFZhelLZvIXeQ2gmyidJXsorRlk13vquV/cPfe1y/F6aG19YXSuvrMSB+du/yOukvqzHoPaV6luq6Dex4tsi+2HkE2UWaWTec/QTZRurKJsstC3WXOjNSVM6Ooph/768BgFjgLWAAAAABJRU5ErkJggg==>

[image3]: <data:image/png;base64,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>