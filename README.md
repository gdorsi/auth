# [WIP] mercurius-auth

![CI workflow](https://github.com/mercurius-js/auth/workflows/CI%20workflow/badge.svg)

**WIP**

Mercurius Auth is a plugin for [Mercurius](https://mercurius.dev) that adds configurable Authentication and Authorization support.

Features:

- 

## Install

```bash
npm i fastify mercurius mercurius-auth
```

## Example

WIP

## Benchmarks

### Normal GraphQL Server Mode | Without Auth

```text
┌─────────┬──────┬──────┬───────┬───────┬─────────┬───────┬────────┐
│ Stat    │ 2.5% │ 50%  │ 97.5% │ 99%   │ Avg     │ Stdev │ Max    │
├─────────┼──────┼──────┼───────┼───────┼─────────┼───────┼────────┤
│ Latency │ 0 ms │ 8 ms │ 17 ms │ 23 ms │ 8.23 ms │ 4 ms  │ 113 ms │
└─────────┴──────┴──────┴───────┴───────┴─────────┴───────┴────────┘
┌───────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┐
│ Stat      │ 1%      │ 2.5%    │ 50%     │ 97.5%   │ Avg     │ Stdev   │ Min     │
├───────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Req/Sec   │ 5483    │ 5483    │ 10855   │ 11071   │ 10364.6 │ 1632.02 │ 5483    │
├───────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Bytes/Sec │ 2.89 MB │ 2.89 MB │ 5.71 MB │ 5.82 MB │ 5.45 MB │ 858 kB  │ 2.88 MB │
└───────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┘

Req/Bytes counts sampled once per second.
114k requests in 10.02s, 60 MB read
```

### Normal GraphQL Server Mode | With Auth

```text
┌─────────┬──────┬──────┬───────┬───────┬─────────┬─────────┬────────┐
│ Stat    │ 2.5% │ 50%  │ 97.5% │ 99%   │ Avg     │ Stdev   │ Max    │
├─────────┼──────┼──────┼───────┼───────┼─────────┼─────────┼────────┤
│ Latency │ 0 ms │ 9 ms │ 19 ms │ 27 ms │ 9.32 ms │ 4.61 ms │ 147 ms │
└─────────┴──────┴──────┴───────┴───────┴─────────┴─────────┴────────┘
┌───────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┐
│ Stat      │ 1%      │ 2.5%    │ 50%     │ 97.5%   │ Avg     │ Stdev   │ Min     │
├───────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Req/Sec   │ 4519    │ 4519    │ 9855    │ 10055   │ 9329.8  │ 1613.39 │ 4518    │
├───────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Bytes/Sec │ 1.28 MB │ 1.28 MB │ 2.79 MB │ 2.85 MB │ 2.64 MB │ 456 kB  │ 1.28 MB │
└───────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┘

Req/Bytes counts sampled once per second.
102k requests in 10.02s, 28.9 MB read
```

## License

MIT
