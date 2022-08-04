# Insert Query

{% hint style="info" %}
Based on MySQL 8.0.28
{% endhint %}

![](<../../../.gitbook/assets/스크린샷 2022-08-01 오후 3.20.39.png>)

dd



![](<../../../.gitbook/assets/스크린샷 2022-08-01 오후 3.18.30 (1).png>)

dd





ibuf0buf.cc

```
#ibuf0buf.cc

static dberr_t ibuf_insert_low (...){

...

err = btr_cur_optimistic_insert(BTR_NO_LOCKING_FLAG | BTR_NO_UNDO_LOG_FLAG,
                                    cursor, &offsets, &offsets_heap, ibuf_entry,
                                    &ins_rec, &dummy_big_rec, thr, &mtr);

    if (err == DB_FAIL) {
      err = btr_cur_pessimistic_insert(
          BTR_NO_LOCKING_FLAG | BTR_NO_UNDO_LOG_FLAG, cursor, &offsets,
          &offsets_heap, ibuf_entry, &ins_rec, &dummy_big_rec, thr, &mtr);
    }
    
...

}
```

* btr\__cur\__optimistic\_insert
* btr\_cur\_pessimistic\_insert

🔼 Insert occurs in these two functions&#x20;





