# Transfers

If you want to transfer money between accounts, you want to do it in a way that doesn't mess up reports. If you only created two transactions, Actual would have no way of knowing they are a single transfer and can be ignored in reports.

When you create a transfer in Actual, those two transactions are linked and updating one always automatically updates the other. For example, if you typed something into the **Notes** column it would appear in both transactions.

## Creating a transfer

In the **Payee** field of a transaction, choose the account in the dropdown you want to transfer to/from. You can press **Make Transfer** if you want to just see a list of accounts and hide other payees.

:::caution
A transaction in the corresponding account will automatically be created.
:::

If you are importing files, it is recommended to import into a single account and create the transfer first, and then import the second account. This way the transaction in the second account is automatically reconciled to the transfer transaction. If you imported to both accounts first, creating the transfer would create a duplicate transaction.

## Deleting a transfer

Delete a transfer the same way you delete any transaction: hover over it and press the **X** on the left. Deleting a transfer transactions always deletes both transactions in each account.

## Transfer Categories

Transfers between On Budget accounts don't have a category.  This is because the funds never left your budget.  One way to think about this is that the funds both left and entered your budget thus canceling each other out. Actual marks these types of transfers with _`Transfer`_ in the category field.

Transfers between Off Budget and On Budget accounts are different.  Only one half of the transfer exists on your budget and, from the perspective of your budget, is the same as a regular transaction.  You can create these transfers just the same as an On Budget transfer, but you will be asked to assign a category on the On Budget side of the transfer.

## Payee rules

Transfers are actually just custom payees, so if you want to you can [create custom rules for them](./payees.md#transfer-payees).
