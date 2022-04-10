# proposal

## Goals:

- We design efficient and performant runtime.
- We maintain clean codebase.
- We maintain linear commit history with clear and semantic commit message.
- We sign every commit.
- We provide Tokio-alike mod interface (this will be considered only after we complete the core part).
- We implement modern linux support.
- We utilize real async IO (via IOUring and Epoll).
- We try our best to reduce dependencies.
- We hope it to be a NUMA-aware job-stealing framework.
- We thrive to give a rich set of features.

## Non Goals:

- We do not expect portability for OS other than Linux.
- We do not provide backward compatibility for ancient kernels before 5.10.
- We do not encourage unsafe hatred. We will try to reduce unsafe blocks only when it can be done without performance compromising. And, [the happiness of coding is much more valuable to us](https://steveklabnik.com/writing/a-sad-day-for-rust).

## Considerations:

- We are not Linux core developers or contributors of liburing. We really welcome any suggestion on performance tuning and we also welcome benchmarks; but we may shutdown any issue if [we think its tone becomes unfriendly for further discussion](https://github.com/axboe/liburing/issues/189). 
- We are open to design corrections. As long as your suggestions are reasonable and well stated, we will never say something like 'Enough, already'.
- We focus on x86-64 for now but leave space for other architectures.
