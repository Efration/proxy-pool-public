# Public proxy list

This repository publishes a list of proxy configurations that were **found,
extracted, and connectivity-tested in private**.

The testing worker, subscription URLs, and project settings are **not** in
this repository. Only the finished list is public.

## `proxies.txt`

[`proxies.txt`](proxies.txt) is the output file. Each line is one proxy
configuration that passed a real protocol-level connectivity test.

Use it as a subscription URL (raw file):

```text
https://raw.githubusercontent.com/YOUR_USER/proxy-pool-public/main/proxies.txt
```

Replace `YOUR_USER` and `proxy-pool-public` with the owner and name of
**this** public repository.

## Config names (`<provider>`)

Every configuration name starts with a provider tag taken from the
subscription link it was extracted from:

```text
<provider>original name
```

Examples:

```text
<youfoundamin>🇩🇪 Germany 01
<iampedi5>🇩🇪 Germany 🚀 Premium
<xrayvip>US-01
```

- The text inside `<...>` is the provider (GitHub owner, or the meaningful
  part of the domain).
- The rest of the name is the original remark, unchanged (flags, emojis,
  spaces, and Unicode are preserved).
- The tag only names the **source subscription**. It is not a ranking, speed
  test, or country check.

## What this list is (and is not)

- Configurations were collected from subscription links, decoded when needed
  (plain URIs, Base64, or sing-box JSON), then tested privately.
- Only configs that succeeded the connectivity test are kept.
- There is no speed ranking and no country detection in this file.
- The list is overwritten when a new private test run finishes.

If a line fails in your client, skip it; the next published update may drop
or replace it.
