# Object-

- Object.keys()
	- 返回一个数组，成员是参数对象自身的（不含继承的）所有可遍历（ enumerable ）属性的键名

		var obj = { foo: "bar", baz: 42 };
	
		Object.keys(obj)
	
		// ["foo", "baz"]

- Object.values()
	- 返回一个数组，成员是参数对象自身的（不含继承的）所有可遍历（ enumerable ）属性的键值。


		var obj = { foo: "bar", baz: 42 };
	
		Object.values(obj)
	
		// ["bar", 42]

- Object.entries
	- 返回一个数组，成员是参数对象自身的（不含继承的）所有可遍历（ enumerable ）属性的键值对数组。


		var obj = { foo: 'bar', baz: 42 };

		Object.entries(obj)

		// [ ["foo", "bar"], ["baz", 42] ]


	Object.entries方法的一个用处是，将对象转为真正的Map结构。

		var obj = { foo: 'bar', baz: 42 };

		var map = new Map(Object.entries(obj));

		map // Map { foo: "bar", baz: 42 }

