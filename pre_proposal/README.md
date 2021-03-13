### Format
Idea
- Elaboration
- Advantages:
- Disadvantages/issues:

## Estimating when a package will be delivered to a given address
- We plan to estimate when a package will be delivered given the carrier, current time of “Out for Delivery”, and address to which it is delivering to.
- When packages are sent out for delivery, the time that they actually get delivered depends on:
	- Route
	- Delivery driver
	- Carrier
	- Size (affects location of delivery (mailbox/door), affects position in linear route)
	- Address (position in linear route)
- Data we need:
	- Name, as an identifier of locatio
	- Courier
	- Mailbox delivery
	- Date of “Out for Delivery”
	- Time of “Out for Delivery”
	- Date of “Delivered”
	- Time of “Delivered”
- ADV:
	- Straightforward to implement
	- Useful (at least for CPR)
- DisADV
	- Data is going to be limited unless we expand our acquisition efforts soon

## Annotating regulatory regions and classifying promoters
- To classify whether certain regulatory regions of genes (potential promoters) are actually being used to initiate transcription
- To be able to expand this to ML algorithms instead of the current state of sticking to HMMs and MCMCs.
- Would need the following information that would need code to extract from each scaffold on each assembly:
