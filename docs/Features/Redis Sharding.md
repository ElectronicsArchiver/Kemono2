
# Redis Sharding

Redis's synchronous nature combined with large, hulking <br>
datasets that require to be scanned repeatedly and often <br>
make for poor scalability.

Let's mitigate those bottlenecks by splitting up the data <br>
Redis has to scan across databases, and entire threads <br>
of execution across instances.

<br>
<br>

## Issues

<br>

-   The  **[`rb`]**  package requires  [`redis` < 3.5][3.5]

<br>


<!----------------------------------------------------------------------------->

[`rb`]: https://github.com/getsentry/rb
[3.5]: https://github.com/getsentry/rb/blob/6f96a68dca2d77e9ac1d8bdd7a21e2575af65a20/setup.py#L15
