---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
contentType: overview
description: Understand trigger nodes in n8n, and browse the trigger nodes library.
---

# Trigger nodes and the trigger library

This section provides information about n8n's trigger nodes and the trigger **nodes library**.

## Trigger nodes

A trigger node starts a workflow and accepts no input from other types of node. You can identify a trigger node by the lightning bolt icon to the left of the node and by the rounded corners on the left hand side of the node.

A trigger node starts a workflow in response to an external event. These external events include those from services, as well as events such as webhooks, [on a schedule](/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger), [AI chat](/integrations/builtin/core-nodes/n8n-nodes-langchain.chattrigger), from [other workflows](/integrations/builtin/core-nodes/n8n-nodes-base.workflowtrigger), and more.

You can also start a workflow with a [manual trigger](/integrations/builtin/core-nodes/n8n-nodes-base.manualworkflowtrigger), which is useful for testing.

/// note
You can only have one manual trigger per workflow.
///

## Triggers library

You can find trigger nodes to add to a workflow in the **node library** when there are no other trigger nodes on the **canvas** or from the **Add another trigger** section of the **node library** when the **canvas** already contains a node.

You can also find triggers for services when browsing [actions](/integrations/builtin/app-nodes) in the **Triggers** section of a service. Many of the service trigger nodes use a combination of webhooks and schedule polling behind the scenes, but provide an simpler interface to work with.

## Moving triggers from testing to production

Using a manual trigger node in combination with the **Test wokflow** button is helpful for manually testing initial workflow design and receiving immediate feedback, but not for other triggers as they don't show feedback in the **canvas**.

Once you activate a workflow, you can see its [executions list](/workflows/executions/) in the **Executions** tab above the workflow canvas.
