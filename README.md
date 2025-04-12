# atls-store

embedded database. zero config.

```rust
use atls_store::DB;

let db = DB::open("data.db")?;
db.put(b"key", b"value")?;
let val = db.get(b"key")?;
```

features:
- acid transactions
- crash recovery
- column families
- ttl support

no servers. no config files. single binary.

inspired by rocksdb but simpler.

[crates.io](https://crates.io/crates/atls-store) • apache-2.0
