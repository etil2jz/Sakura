
[website]: https://bloom.host
[discord]: https://discord.gg/bloom
[release]: https://github.com/etil2jz/Sakura/releases

<img src="sakura-logo.webp" alt="sakura_logo" width="80" height="80">

# Sakura Performance Minecraft JAR

Sakura is a performance-oriented fork of Purpur intended to increase performance for entity-heavy servers by implementing multi-threaded and asynchronous improvements.

Those improvements are directly backported from [Petal](https://github.com/Bloom-host/Petal), the 1.19.2 version.

## Sponsored by Bloom Host

<img src="https://bloom.host/assets/images/logo-white.svg" alt="bloom_logo" width="240" height="80">

Development of Petal is sponsored by [Bloom Host][website], your home for the highest performance dedicated-core Minecraft hosting, VPS hosting, and bare metal dedicated servers. Bloom serves thousands of customers across the world with locations in Virginia, Dallas, Los Angeles, Miami, Germany, and soon to be Singapore! 

Join the [Bloom Host discord][discord] to connect with over 4,000 members and learn more about their services. Petal ticket support is limited to customers of Bloom Host, but a community support channel is available in the Bloom discord for anybody to use.

For a limited time, you can enjoy 15% off your first invoice for any Minecraft/VPS hosting product with the coupon code `PETALPOWER`

## Features

Sakura focuses on two specific improvements for entity-heavy servers:

- **Async Pathfinding** Entity pathfinding is offloaded to asynchronous threads to significantly reduce processing from the main thread
- **Multi-threaded Entity Tracking** Entity tracking can take advantage of multiple threads to greatly reduce dependence on main thread processing


As Sakura is forked from Purpur, it enjoys several performance features from other projects including:

- **Sentry Integration** Easily track all errors coming from your server in excruciating detail (Pufferfish)
- **Better Entity Performance** Reduces the performance impact of entities by skipping useless work and making barely-noticeable changes to behavior (Pufferfish)
- **Partial Asynchronous Processing** Partially offloads some heavy work to other threads where possible without sacrificing stability (Pufferfish)
- **8x Faster Map Rendering** Reduces or eliminates lag spikes caused by plugins like ImageOnMap or ImageMaps (Pufferfish)
- **30% faster hoppers** over Paper (Airplane)
- **Reduced GC times & frequency** from removing useless allocations, which also improves CPU performance (Airplane)
- **Fast raytracing** which improves performance of any entity which utilizes line of sight, mainly Villagers (Airplane)
- **Built-in profiler** which has 0 performance hit and easy to read metrics for both server owners and developers (Airplane)

## Testimonials

> Petal has significantly improved entity performance on our 1.19 servers such as survival & skyblock. This has allowed us to increase per player mob spawn caps & increase frequency of mob spawning without having to worry about taking a performance hit.

-Foxcraft

## Download

The latest JAR can currently be found on the releases page [here][release].

## License

Sakura is licensed under GPLv3.
