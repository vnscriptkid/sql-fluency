## Item 9: Denormalization for information warehouse
- use cases:
    - need faster reads (by storing dupliate data to avoid join), in read-intensive app
    - not losing history: invoice data must hold address of user at the time he made the order, not current address
    - calculated data: keep total in invoice