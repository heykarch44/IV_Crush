# CoreWeave (CRWV) Sympathy Trade Strategy Blueprint

## 1. Trade Catalyst
* **Macro Event:** Nebius (NBIS) secured a massive $2.6 Billion AI data center infrastructure agreement. 
* **Sympathy Mechanics:** CRWV serves as the direct "Neocloud" competitor to NBIS. Capital is rotating into CRWV to front-run the validation of massive demand for AI infrastructure and GPU power grids.

## 2. Option Parameter Selection (The Sweet Spot)
* **Runway Window:** June 18, 2026 Expiration (~4 weeks out). Avoids the high-theta bleed of weekly options while preserving strong near-term leverage.
* **Strike Target:** $105.00 At-The-Money (ATM) or $100.00 In-The-Money (ITM).
* **Greek Advantage:** The $105 Call features a low Implied Volatility (IV) Percentile of 21.3% (historically cheap options) and a dense 0.65+ Delta.

## 3. Trade Execution Rules

### Phase A: Entry Order
* **Order Type:** Limit Order only. Never use Market Orders.
* **Pricing Action:** Check the active Bid and Ask (e.g., $6.50 Bid / $6.80 Ask) and find the mathematical midpoint ($6.65). Place a resting limit buy order right at the mid-price to eliminate the $0.30 market maker spread tax.

### Phase B: Protection (The Underlying Stock Trigger)
Do not set standard stop-loss orders based on the option's premium value. Instead, configure a ThinkOrSwim **Conditional Order** linked directly to the equity chart:
* **Trigger Constraint:** Stock Price of CRWV is Less Than or Equal To (<=) $102.95 (just below the defined morning intraday support floor of $103.16).
* **Routing Action:** If triggered, automatically route a Market Order to Sell to Close the active June Call contracts.
