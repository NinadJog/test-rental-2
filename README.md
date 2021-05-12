# test-rental-2

## Daml smart contracts for home rentals

The program has two logical parts. The first part uses the Propose and Accept design pattern for the landlord to propose a rental and for a prospective tenant to accept or reject it.

If the prospective tenant accepts it, the landlord provides a second contract containing the logistics of the monthly rent payment.

The landlord is the signatory on all contracts while the tenant is an observer. The template for payment logistics provides choices to the tenant for determining the balance due and for paying rent.

There is a 10% penalty if the tenant pays rent late, after the 5th of the month, but these rental terms, including the monthly rent, can be changed at the outset by the landlord.

The main purpose for writing this program was to get a feel for Daml syntax and contract semantics rather than to faithfully mimic real-world interactions.
