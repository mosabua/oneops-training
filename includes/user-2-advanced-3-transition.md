# Transition

> Environments, Clouds and More in Depth

<!--- vertical -->

## Environments

Allow usage of same design for different purposes

- scale
- availability
- cloud usage
- dns
- and component configuration!

Note:
- review override lock and such

<!--- vertical -->

## Cloud Characteristics

In OneOps:

- primary /  secondary / unused
- deployment order
- scale

In underlying cloud provider:

- available instance types
- available operating systems
- available services
- ... 

<!--- vertical -->

## Cloud Selection

- Primary:
  - Use cloud now
- Secondary:
  - Maybe use cloud later
  - _Disables_ the traffic
- Order:
  - Sequence of release deployments
  - Important for roll out
- Scale:
  - Increases/decrease the number of instances

Configure __per environment at creation!__

Note:
- Demo environment creation with cloud selection and show

<!--- vertical -->

## Cloud Configuration and Changes

- Make Primary/Secondary
  - Enable/disable traffic
- Ignore: 
  - Changes _do not_ apply
- Shutdown: 
  - _Decommission_ all the resources
  - Easily turn on again
- Change order and scale

Configure __per environment per platform in transition!__

Note:
- Demo cloud operations in transition (see above)
- and in operation (autorepair on/off)

<!--- vertical -->

## Best Practices

- 2 x 2 x 2
  - But possible to run in one cloud at a time
- Auto repair and auto replace on
  - with suitable times set up
- Configure smart ECV checks
- Expect _failure_ 
  - reboot possible any time
  - cloud and VM maintenance
  - real failures

<!--- vertical -->

## 2 x 2 x 2 Minimum

What does that mean?

- 2 computes per platform
- 2 clouds
- 2 data centers

Internal, non-critical applications can be 2x1x2.

Typical customer facing applications way more.

Note:
Minimum - large systems can have 8 or more clouds 

<!--- vertical -->

## Practices to Avoid

- Dependency on specific rack, hardware, ...
- No reliance on specific VMs = no pets!
- No IP number usage

<!--- vertical -->

## Rolling out Changes

- Pack pull in design
- Design change
- Design pull in transition
- Configuration change in transition

All are __committed__ and __create a release__,

and in transition __create a deployment__.

<!--- vertical -->

## Destructive Changes

- Removed platform
- Removed component
- Removed config
- Delete cloud
- Reduced scale

Again, all are __committed__ and __create a release__,

and in transition __create a deployment__.

<!--- vertical -->

## Questions? 

<em class="yellow">Ask now, before we jump to the next section.</em>
