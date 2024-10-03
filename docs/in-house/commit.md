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

    If, after accounting for fees and errors, there is still a mismatch between the projected amount in the DGP packet and the actual running total in RE, it is essential to know how to find the source of the discrepancy. Here is a list of common issues and the way to diagnose them:

    - **Problem:** Incorrect gift amounts
        - **Solution:** Verify that you entered all gift amounts correctly and that you did not, for instance, move a decimal place in one of the gifts.
    - **Problem:** Missing Fees
        - **Solution:** Ensure that you have captured and accounted for all 3PW fees. You can verify this by either examining the total 3PW gift amount vs. the check amount issued in the distribution, or by going into the distribution breakdown spreadsheet and looking for a `Fees` column.
    - **Problem:** Missing gifts
        - **Solution:** Export your batch to a grid and open in excel. First, process your data to recombine gifts that are a part of the same check. For example, you could *FILTER* by the `Check Number` column for unique values, and then perform a *SUMIF* to get the total of all gifts under that check number. Then, compare all the gift totals in batch to those listed on page 2 of the DGP packet. The easiest way to identify discrepancies could be to put the expected DGP gifts into the spreadsheet as well, sort both columns by amount, and then see whether the batch or the packet is missing gifts. *If the packet is missing gifts, see "DGP Packet Missing Gifts" below.*

??? danger "DGP Packet Missing Gifts"

    If the **DGP Packet** is missing gifts, it is important to notify DRC so they can correct the packet. The gift may have either been forgotten, or intentionally excluded from the packet, so they will need to update the packet accordingly before you can proceed with the batch.

### Update the Projected Gift Amount and Number of Gifts

1. Open the **Gift Batch Setup** menu.
2. Update the `Projected Number of Gifts` field with the *Running Total*.
3. Update the `Project Amount` field with the *Running Total* number of gifts.

## Audit Process

1. When you are ready, commit the batch.
2. Navigate to your Raiser's Edge **Home** page where your favorite queries should be stored.
3. Perform the standard batch audits and validation processes by using the **Address Accelerator** and the queries saved to your Home page.
4. Move the Asana batch into **Receipting**.
5. Select the *Summary for DGP* query and enter the batch number into the query wizard.
6. Export the generated document to a PDF and then open it.
    1. **Note:** As of the time of writing, it is better to open the PDF from your local File Select, instead of opening it when prompted by Raiser's Edge after exporting it.
7. If it is not already open, open the gift packet for this batch as well.
8. Insert the *Summary for DGP* document as the second page of the DGP packet, and then save the DGP packet.
9. Rename the DGP packet to *Batch Date - DONE Initials Batch Number*.
10. Move the DGP packet to:

```text
S:\FISCAL - Docs from Development\Digital Gift Packet\DoTS Final
```
