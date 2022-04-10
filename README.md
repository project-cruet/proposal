# proposal

## Goals:

- We design efficient and performant runtime.
- We maintain clean codebase.
- We maintain linear commit history with clear and semantic commit message.
- We sign every commit.
- We provide Tokio-alike mod interface (this will be considered only after we complete the core part).
- We implement modern linux support.
- We utilize real async IO (via IOUring and Epoll).
- We try out best to reduce dependencies.
- We hope it to be a NUMA-aware job-stealing framework.
- We thrive to give a rich set of features.

## Non Goals:

- We do not expect portabiliy for OS other than Linux is not a goal.
- We do not provide backward compatibility for acient kernels before 5.10.
- We do not encourage unsafe hatred. We will try to reduce unsafe blocks only when it can be done without performance compromising. And, [the happiness of coding is much more valuable to us](https://steveklabnik.com/writing/a-sad-day-for-rust)

## Considerations:

- We are not Linux core developpers or contributors of liburing. We really welcome any suggestion on performance tuning and we also welcome benchmarks; but we may shutdown any issue if [we think its tone becomes unfriendly for further discussion](https://github.com/axboe/liburing/issues/189). 
