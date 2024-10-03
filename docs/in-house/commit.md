# Commit and Audit

## Modify Expected Amounts

For context, it is necessary to update the expected amounts in batch because they will likely differ from what was expected in the DAA packet due to 3PW gifts and fees. It is important to update the expected number of gifts with the actual number of gifts received, and verify that the batch gift amount, adjusted for fees, matches the expected amount.

??? info "More on how 3PW gifts affect batch totals"

    When we receive a distribution from a 3PW platform, we receive a single check via the 3PW vehicle for the total amount of all gifts combined, minus any fees they may apply. Many 3PW distributions will also come with instructions to access their web portal that contains a distribution breakdown of all donors and individual amount donated. When we have access to these distributions, we enter them in batch as separate gifts using the original amount (not including fees) given by each donor. Therefore, this process will *inflate* both the number of gifts as well as the total dollar value received in a batch.

### Verify Batch Running Total

1. Locate the Batch **Running Total** in the bottom right corner of the Batch window.
2. If you do not already have it open, open the DAA gift packet for this in house batch.
3. Locate the expected RE amount on the first page of the packet in the **TOTAL DONATIONS = RE** line item.
4. Verify that **Running Total - Fees = TOTAL DONATIONS = RE**.
5. If the totals match, add a sticky note in the packet next to the **TOTAL DONATIONS = RE** line item with the following information:
    1. **Actual RE Total:** $ *Running Total*
    2. **3PW Fees:** $ *3PW fee amount*

??? warning "Tips on diagnosing mismatched projected amount and running totals"

    Lorem ipsum

### Update the Projected Gift Amount and Number of Gifts

1. Open the **Gift Batch Setup** menu.
2. Update the `Projected Number of Gifts` field with the *Running Total*.
3. Update the `Project Amount` field with the *Running Total* number of gifts.
