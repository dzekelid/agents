---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Withdraw funds for the agent
  version: 1.0.0
  description: Withdraw funds for the agent.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accountingsystem/agentcash:
    get:
      summary: Gets overview of the agent cash account
      description: Gets overview of the agent cash account.
      operationId: AccountingSystem_GetAgentCash
      x-api-path-slug: apiaccountingsystemagentcash-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Overview
      - Of
      - Agent
      - Cash
      - Account
  /api/invoice/fees:
    get:
      summary: Get agent fees invoices earned
      description: Get agent fees invoices earned.
      operationId: Invoice_GetAgentFeesEarned
      x-api-path-slug: apiinvoicefees-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Agent
      - Fees
      - Invoices
      - Earned
  /api/locale/{culture}:
    get:
      summary: returns the json file containing localization for the app based on
        a culture string, and any custom values for the agent
      description: Returns the json file containing localization for the app based
        on a culture string, and any custom values for the agent.
      operationId: Locale_GetLocalisationFileByculture
      x-api-path-slug: apilocaleculture-get
      parameters:
      - in: path
        name: culture
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Json
      - File
      - Containing
      - Localizationthe
      - App
      - Based
      - "On"
      - Culture
      - String
      - ""
      - Any
      - Custom
      - Valuesthe
      - Agent
  /api/posting/cash:
    get:
      summary: Get all postings in the cash account for the agent
      description: Get all postings in the cash account for the agent.
      operationId: Posting_GetCashFunds
      x-api-path-slug: apipostingcash-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Postings
      - In
      - Cash
      - Accountthe
      - Agent
  /api/receipt/agentdeposit:
    post:
      summary: Add agent funds into the system
      description: Add agent funds into the system.
      operationId: Receipt_ReceiptAgentDepositByagentDepositDataContract
      x-api-path-slug: apireceiptagentdeposit-post
      parameters:
      - in: body
        name: agentDepositDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Agent
      - Funds
      - Into
      - System
  /api/receipt/withdrawfunds:
    post:
      summary: Withdraw funds for the agent
      description: Withdraw funds for the agent.
      operationId: Receipt_WithdrawFundsBywithdrawFundsDataContract
      x-api-path-slug: apireceiptwithdrawfunds-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawFundsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Withdraw
      - Fundsthe
      - Agent
  /api/tax/agentheld:
    get:
      summary: Get all tax held by agent
      description: Get all tax held by agent.
      operationId: Tax_GetAgentTaxHeldLedger
      x-api-path-slug: apitaxagentheld-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tax
      - Held
      - By
      - Agent
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---