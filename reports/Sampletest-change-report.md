# CPI Change Report - Sampletest

**Generated On:** Sat May 16 17:19:13 UTC 2026

## Changed File Summary

Changes detected.

```text
Files old-unzip/metainfo.prop and new-unzip/metainfo.prop differ
Only in new-unzip/src/main/resources: parameters.prop
Only in new-unzip/src/main/resources: parameters.propdef
Files old-unzip/src/main/resources/scenarioflows/integrationflow/Sampletest.iflw and new-unzip/src/main/resources/scenarioflows/integrationflow/Sampletest.iflw differ
```

## Detailed Diff

```diff
diff -ru old-unzip/metainfo.prop new-unzip/metainfo.prop
--- old-unzip/metainfo.prop	2026-05-14 04:20:22.000000000 +0000
+++ new-unzip/metainfo.prop	2026-05-16 17:19:12.000000000 +0000
@@ -1,3 +1,3 @@
 #Store metainfo properties
-#Thu May 14 04:20:23 UTC 2026
+#Sat May 16 17:19:13 UTC 2026
 description=
Only in new-unzip/src/main/resources: parameters.prop
Only in new-unzip/src/main/resources: parameters.propdef
diff -ru old-unzip/src/main/resources/scenarioflows/integrationflow/Sampletest.iflw new-unzip/src/main/resources/scenarioflows/integrationflow/Sampletest.iflw
--- old-unzip/src/main/resources/scenarioflows/integrationflow/Sampletest.iflw	2026-05-14 04:20:22.000000000 +0000
+++ new-unzip/src/main/resources/scenarioflows/integrationflow/Sampletest.iflw	2026-05-16 17:19:12.000000000 +0000
@@ -1,13 +1,16 @@
-<?xml version="1.0" encoding="UTF-8"?><bpmn2:definitions xmlns:bpmn2="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" xmlns:ifl="http:///com.sap.ifl.model/Ifl.xsd" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" id="Definitions_1" name="Definitions 1" targetNamespace="http://com.sap.it.ifl.tooling/default/flow">
+<?xml version="1.0" encoding="UTF-8"?><bpmn2:definitions xmlns:bpmn2="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" xmlns:ifl="http:///com.sap.ifl.model/Ifl.xsd" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" id="Definitions_1">
     <bpmn2:collaboration id="Collaboration_1" name="Default Collaboration">
-        <bpmn2:documentation id="Documentation_1440568604517" textFormat="text/plain"/>
         <bpmn2:extensionElements>
             <ifl:property>
-                <key>cmdVariantUri</key>
-                <value>ctype::IFlowVariant/cname::IFlowConfiguration/version::1.2.4</value>
-        	</ifl:property>
+                <key>namespaceMapping</key>
+                <value/>
+            </ifl:property>
+            <ifl:property>
+                <key>httpSessionHandling</key>
+                <value>None</value>
+            </ifl:property>
             <ifl:property>
-                <key>privateKeyAlias</key>
+                <key>accessControlMaxAge</key>
                 <value/>
             </ifl:property>
             <ifl:property>
@@ -15,40 +18,48 @@
                 <value>false</value>
             </ifl:property>
             <ifl:property>
-                <key>traceLevel</key>
-                <value/>
+                <key>log</key>
+                <value>All events</value>
             </ifl:property>
             <ifl:property>
-                <key>ServerTrace</key>
+                <key>corsEnabled</key>
                 <value>false</value>
             </ifl:property>
             <ifl:property>
-                <key>namespaceMapping</key>
+                <key>exposedHeaders</key>
                 <value/>
             </ifl:property>
             <ifl:property>
-                <key>errorStrategy</key>
-                <value/>
+                <key>componentVersion</key>
+                <value>1.2</value>
             </ifl:property>
             <ifl:property>
                 <key>allowedHeaderList</key>
                 <value/>
             </ifl:property>
             <ifl:property>
-                <key>httpSessionHandling</key>
-                <value>None</value>
+                <key>ServerTrace</key>
+                <value>false</value>
             </ifl:property>
             <ifl:property>
-                <key>corsEnabled</key>
-                <value>false</value>
+                <key>allowedOrigins</key>
+                <value/>
             </ifl:property>
             <ifl:property>
                 <key>accessControlAllowCredentials</key>
                 <value>false</value>
             </ifl:property>
             <ifl:property>
-                <key>componentVersion</key>
-                <value>1.2</value>
+                <key>allowedHeaders</key>
+                <value/>
+            </ifl:property>
+            <ifl:property>
+                <key>allowedMethods</key>
+                <value/>
+            </ifl:property>
+            <ifl:property>
+                <key>cmdVariantUri</key>
+                <value>ctype::IFlowVariant/cname::IFlowConfiguration/version::1.2.4</value>
             </ifl:property>
         </bpmn2:extensionElements>
         <bpmn2:participant id="Participant_1" ifl:type="EndpointSender" name="Sender">
@@ -61,14 +72,6 @@
                     <key>ifl:type</key>
                     <value>EndpointSender</value>
                 </ifl:property>
-                <ifl:property>
-                    <key>cmdVariantUri</key>
-                    <value>ctype::FlowstepVariant/cname::Sender/version::1.0</value>
-        		</ifl:property>
-                <ifl:property>
-                    <key>componentVersion</key>
-                    <value>1.0</value>
-                </ifl:property>
             </bpmn2:extensionElements>
         </bpmn2:participant>
         <bpmn2:participant id="Participant_2" ifl:type="EndpointRecevier" name="Receiver">
@@ -77,14 +80,6 @@
                     <key>ifl:type</key>
                     <value>EndpointRecevier</value>
                 </ifl:property>
-                <ifl:property>
-                    <key>cmdVariantUri</key>
-                    <value>ctype::FlowstepVariant/cname::Receiver/version::1.0</value>
-        		</ifl:property>
-                <ifl:property>
-                    <key>componentVersion</key>
-                    <value>1.0</value>
-                </ifl:property>
             </bpmn2:extensionElements>
         </bpmn2:participant>
         <bpmn2:participant id="Participant_Process_1" ifl:type="IntegrationProcess" name="Integration Process" processRef="Process_1">
@@ -94,10 +89,6 @@
     <bpmn2:process id="Process_1" name="Integration Process">
         <bpmn2:extensionElements>
             <ifl:property>
-                <key>cmdVariantUri</key>
-                <value>ctype::FlowElementVariant/cname::IntegrationProcess/version::1.2.1</value>
-        	</ifl:property>
-            <ifl:property>
                 <key>transactionTimeout</key>
                 <value>30</value>
             </ifl:property>
@@ -106,6 +97,10 @@
                 <value>1.2</value>
             </ifl:property>
             <ifl:property>
+                <key>cmdVariantUri</key>
+                <value>ctype::FlowElementVariant/cname::IntegrationProcess/version::1.2.1</value>
+            </ifl:property>
+            <ifl:property>
                 <key>transactionalHandling</key>
                 <value>Not Required</value>
             </ifl:property>
@@ -113,53 +108,130 @@
         <bpmn2:endEvent id="EndEvent_2" name="End">
             <bpmn2:extensionElements>
                 <ifl:property>
-                    <key>cmdVariantUri</key>
-                    <value>ctype::FlowstepVariant/cname::MessageEndEvent/version::1.1.0</value>
-        		</ifl:property>
-                <ifl:property>
                     <key>componentVersion</key>
                     <value>1.1</value>
                 </ifl:property>
+                <ifl:property>
+                    <key>cmdVariantUri</key>
+                    <value>ctype::FlowstepVariant/cname::MessageEndEvent/version::1.1.0</value>
+                </ifl:property>
             </bpmn2:extensionElements>
-            <bpmn2:incoming>SequenceFlow_3</bpmn2:incoming>
+            <bpmn2:incoming>SequenceFlow_7</bpmn2:incoming>
             <bpmn2:messageEventDefinition/>
         </bpmn2:endEvent>
-        <bpmn2:startEvent id="StartEvent_2" name="Start">
+        <bpmn2:callActivity id="CallActivity_4" name="Content Modifier ">
             <bpmn2:extensionElements>
                 <ifl:property>
+                    <key>bodyType</key>
+                    <value>constant</value>
+                </ifl:property>
+                <ifl:property>
+                    <key>propertyTable</key>
+                    <value/>
+                </ifl:property>
+                <ifl:property>
+                    <key>headerTable</key>
+                    <value/>
+                </ifl:property>
+                <ifl:property>
+                    <key>wrapContent</key>
+                    <value>hello</value>
+                </ifl:property>
+                <ifl:property>
+                    <key>componentVersion</key>
+                    <value>1.6</value>
+                </ifl:property>
+                <ifl:property>
+                    <key>activityType</key>
+                    <value>Enricher</value>
+                </ifl:property>
+                <ifl:property>
                     <key>cmdVariantUri</key>
-                    <value>ctype::FlowstepVariant/cname::MessageStartEvent/version::1.0</value>
-        		</ifl:property>
+                    <value>ctype::FlowstepVariant/cname::Enricher/version::1.6.3</value>
+                </ifl:property>
+            </bpmn2:extensionElements>
+        </bpmn2:callActivity>
+        <bpmn2:callActivity id="CallActivity_6" name="Content Modifier 1">
+            <bpmn2:extensionElements>
+                <ifl:property>
+                    <key>bodyType</key>
+                    <value>constant</value>
+                </ifl:property>
+                <ifl:property>
+                    <key>propertyTable</key>
+                    <value/>
+                </ifl:property>
+                <ifl:property>
+                    <key>headerTable</key>
+                    <value/>
+                </ifl:property>
+                <ifl:property>
+                    <key>wrapContent</key>
+                    <value/>
+                </ifl:property>
+                <ifl:property>
+                    <key>componentVersion</key>
+                    <value>1.6</value>
+                </ifl:property>
+                <ifl:property>
+                    <key>activityType</key>
+                    <value>Enricher</value>
+                </ifl:property>
+                <ifl:property>
+                    <key>cmdVariantUri</key>
+                    <value>ctype::FlowstepVariant/cname::Enricher/version::1.6.3</value>
+                </ifl:property>
+            </bpmn2:extensionElements>
+            <bpmn2:incoming>SequenceFlow_3</bpmn2:incoming>
+            <bpmn2:outgoing>SequenceFlow_7</bpmn2:outgoing>
+        </bpmn2:callActivity>
+        <bpmn2:startEvent id="StartEvent_2" name="Start">
+            <bpmn2:extensionElements>
                 <ifl:property>
                     <key>componentVersion</key>
                     <value>1.0</value>
                 </ifl:property>
+                <ifl:property>
+                    <key>cmdVariantUri</key>
+                    <value>ctype::FlowstepVariant/cname::MessageStartEvent/version::1.0</value>
+                </ifl:property>
             </bpmn2:extensionElements>
             <bpmn2:outgoing>SequenceFlow_3</bpmn2:outgoing>
             <bpmn2:messageEventDefinition/>
         </bpmn2:startEvent>
-        <bpmn2:sequenceFlow id="SequenceFlow_3" sourceRef="StartEvent_2" targetRef="EndEvent_2"/>
+        <bpmn2:sequenceFlow id="SequenceFlow_7" sourceRef="CallActivity_6" targetRef="EndEvent_2"/>
+        <bpmn2:sequenceFlow id="SequenceFlow_3" sourceRef="StartEvent_2" targetRef="CallActivity_6"/>
     </bpmn2:process>
     <bpmndi:BPMNDiagram id="BPMNDiagram_1" name="Default Collaboration Diagram">
         <bpmndi:BPMNPlane bpmnElement="Collaboration_1" id="BPMNPlane_1">
-            <bpmndi:BPMNShape bpmnElement="Participant_1" id="BPMNShape_Participant_1">
-                <dc:Bounds height="140.0" width="100.0" x="40.0" y="100.0"/>
+            <bpmndi:BPMNShape bpmnElement="EndEvent_2" id="BPMNShape_EndEvent_2">
+                <dc:Bounds height="32.0" width="32.0" x="703.0" y="142.0"/>
+            </bpmndi:BPMNShape>
+            <bpmndi:BPMNShape bpmnElement="StartEvent_2" id="BPMNShape_StartEvent_2">
+                <dc:Bounds height="32.0" width="32.0" x="292.0" y="142.0"/>
             </bpmndi:BPMNShape>
             <bpmndi:BPMNShape bpmnElement="Participant_2" id="BPMNShape_Participant_2">
                 <dc:Bounds height="140.0" width="100.0" x="900.0" y="100.0"/>
             </bpmndi:BPMNShape>
-            <bpmndi:BPMNShape bpmnElement="StartEvent_2" id="BPMNShape_StartEvent_2">
-                <dc:Bounds height="36.0" width="36.0" x="292.0" y="142.0"/>
+            <bpmndi:BPMNShape bpmnElement="CallActivity_4" id="BPMNShape_CallActivity_4">
+                <dc:Bounds height="60.0" width="100.0" x="431.0" y="120.0"/>
             </bpmndi:BPMNShape>
-            <bpmndi:BPMNShape bpmnElement="EndEvent_2" id="BPMNShape_EndEvent_2">
-                <dc:Bounds height="36.0" width="36.0" x="703.0" y="142.0"/>
+            <bpmndi:BPMNShape bpmnElement="Participant_1" id="BPMNShape_Participant_1">
+                <dc:Bounds height="140.0" width="100.0" x="58.0" y="72.0"/>
             </bpmndi:BPMNShape>
             <bpmndi:BPMNShape bpmnElement="Participant_Process_1" id="BPMNShape_Participant_Process_1">
-                <dc:Bounds height="220.0" width="540.0" x="250.0" y="60.0"/>
+                <dc:Bounds height="220.0" width="569.0" x="250.0" y="60.0"/>
+            </bpmndi:BPMNShape>
+            <bpmndi:BPMNShape bpmnElement="CallActivity_6" id="BPMNShape_CallActivity_6">
+                <dc:Bounds height="60.0" width="100.0" x="566.0" y="128.0"/>
             </bpmndi:BPMNShape>
-            <bpmndi:BPMNEdge bpmnElement="SequenceFlow_3" id="BPMNEdge_SequenceFlow_3" sourceElement="BPMNShape_StartEvent_2" targetElement="BPMNShape_EndEvent_2">
-                <di:waypoint x="323.5" xsi:type="dc:Point" y="158.0"/>
-                <di:waypoint x="703.5" xsi:type="dc:Point" y="158.0"/>
+            <bpmndi:BPMNEdge bpmnElement="SequenceFlow_3" id="BPMNEdge_SequenceFlow_3" sourceElement="BPMNShape_StartEvent_2" targetElement="BPMNShape_CallActivity_6">
+                <di:waypoint x="308.0" xsi:type="dc:Point" y="158.0"/>
+                <di:waypoint x="616.0" xsi:type="dc:Point" y="158.0"/>
+            </bpmndi:BPMNEdge>
+            <bpmndi:BPMNEdge bpmnElement="SequenceFlow_7" id="BPMNEdge_SequenceFlow_7" sourceElement="BPMNShape_CallActivity_6" targetElement="BPMNShape_EndEvent_2">
+                <di:waypoint x="616.0" xsi:type="dc:Point" y="158.0"/>
+                <di:waypoint x="719.0" xsi:type="dc:Point" y="158.0"/>
             </bpmndi:BPMNEdge>
         </bpmndi:BPMNPlane>
     </bpmndi:BPMNDiagram>
```
