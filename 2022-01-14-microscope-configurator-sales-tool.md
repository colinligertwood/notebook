# Scheduling build times for configurator driven sales.

2022-01-14
Lana, Colin L.

## Colin's Notes

Why can't we use a higher order product to combine microscope parts?
- Anything that's configurator driven can create endless part combinations.
- Want to avoid linking serial numbers together. A microscope is meant to be reconfigured.
- By nature, these are separate products. They're just assembled together, and shipped in the same box.

Is this product bundling?
- Yes. All of these things need to be built, and then shipped together on an order.
- No. We don't want to have a single part number that represents the bundle.
- Yes. There's a top-line service that represents bundling/assembly.

Current dashboard issues?
- Customer items shows products being due on their ship date. This doesn't account for the need for final steps such as calibration. All of that is currently
- We need to be able to display a build-by date that takes into account the leadtime for the assembly/etc. service. This needs to be displayed correctly on th
- Build-by dates are currently incorrect. There needs to be some way to flag that an order depends on a bundle so production pays attention to the build-by da
  - Fixing build-by date so that it's a number that makes sense for everything will also take care of it.

Configurator output?
- Configurator outputs a list of products that are required for the order. The products go into a cart which can be pulled into Zerp.
- It gets pulled into a sales order (Yahya can go into more detail).
- A note is included with the cart ID number from the configurator/website.

Could sales order line grouping/combined lines possibly work to combine products into a bundle?
- Yes.
- No. We don't want to have a single part number that represents the bundle.
- Confirm whether combined lines will work.
- Can combined lines checks be disabled for just these products?
  - The N.0 of the product could be the product assembly/bundling service.
  - Use of this product as the N.0 of the grouping could allow any product to be included in the group.
  - This product would be a service.
- Can a bundle built with combined-lines be displayed on a sales order without combining lines into a single part number?
- Maybe another type of grouping field on sales order liness will be necessary.

## Next steps

- Loop Yahya in, and get his input on whether this could be handled with sales orders, grouping, and build-by dates.
- Loop Virginia in, and get her input on whether these requirements can be met using existing production dashboards.

