# Examples

<figure>

<pre class="diagram mermaid">

flowchart TD
  activity-1[:activity-1] -->|prov:used| entity-1(["`:entity-1
  schema:identifier 'xyz'`"])
  style entity-1 fill:#FFFFCC,stroke:#FFFF33
  entity-1 -->|prov:wasGeneratedBy| activity-1
  activity-2[:activity-2] -->|prov:wasInformedBy| activity-1
  activity-2 -->|prov:used| entity-1
  activity-3[:activity-3] -->|prov:wasInformedBy| activity-2
  activity-3 -->|prov:used| entity-1
  activity-4[:activity-4] -->|prov:wasInformedBy| activity-3
  activity-4 -->|prov:used| entity-1

</pre>

<figcaption>Use of prov:Entity to create an affair identifier.</figcaption>

</figure>