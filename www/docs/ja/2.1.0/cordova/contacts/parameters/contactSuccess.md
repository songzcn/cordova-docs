---
license: >
    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.

title: contactSuccess
---

contactSuccess
==============

`[contacts.find](../contacts.find.html)` メソッドの実行に成功した場合に呼び出される、 `[Contact](../Contact/contact.html)` 配列を提供するコールバック関数です。

    function(contacts) {
        // 任意のコード
    }

パラメーター
----------

- __contacts:__ 検索の結果の連絡先配列 (`[Contact](../Contact/contact.html)`)

[使用例](../../storage/storage.opendatabase.html)
-------

    function contactSuccess(contacts) {
        for (var i=0; i<contacts.length; i++) {
            console.log("表示名 = " + contacts[i].displayName);
        }
    }
