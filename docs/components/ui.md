---
id: pidmr_ui
title: Metaresolver UI
sidebar_position: 3
---

### Metaresolver UI -  PIDMR-UI

The Metaresolver UI (PIDMR-UI) is a web-application, created using the React javascript framework. Metaresolver UI provides the main user 
interface for resolving PIDs. It is the first client that validates and tests the use of the Metaresolver API. The current development 
instance resides at [pidmr.argo.grnet.gr](pidmr.argo.grnet.gr) and uses the Metaresolver API (PIDMR-API)  as backend.

The UI consists of two main views:

 - The persistent identifier resolver UI: In this view the user can enter a PID of any of the supported types and choose to resolve it in one of three ways: a) Get PID's landing page b) Get PID's metadata, c) Get PID's resource itself.  For each Provider the  Metaresolver UI supports one or many of the above resolving modes. The Metaresolver UI also includes an informational box which responds interactively to the user input and displays information about the current input and suggestions. This is a library of persistent identifiers that tries to help the end user understand the use of PIDs,  validates the PID before resolving it and guides the user on how to correctly use it.
 - Supported Providers : In this view the UI displays a dynamic list (retrieved from the backend api) with all Supported PID Providers / PID types. Currently this page presents the following information a) name/prefix used b) short description, c) supported resolving modes
 - Documentation of the process: In this view the UI displays the process a provider should follow.
 - 

