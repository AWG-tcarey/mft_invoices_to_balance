# mft_invoices_to_balance
---
## Build Data
--- _Information below this line is used by the deploy process. Please **triple-check** for spelling errors!_ ---
### Actions
- aislprod/lin_MQ_integration/get_freight_invoices_for_bal
    - %data%/aislprod/sentbox/freightinv/
    - %data%/aislprod/outbox/invoices/    
    - %aislprod%/inbound/freightinv/
- aislprod/lin_MQ_integration/put_bal_invoices_to_merged
    - %data%/aislprod/receivedbox/invoices/
- awg.supplychainproducts.com/balances/put_bal_merged_invoices
- service_trhapp/move_bal_edi_invoice
    - %data%/receivedbox/edi/
    - %prhappftpuserdata%/inbox/edi/
    - %data%/aislprod/outbox/invoices/
