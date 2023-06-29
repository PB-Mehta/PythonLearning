Q1. The main difference between `__getattr__` and `__getattribute__` is in their behavior and the stage at which they are invoked:
- `__getattr__` is only called when an attribute is not found through normal lookup in the instance, its class, or any of its superclasses. It is invoked as a fallback mechanism when attribute access fails.
- `__getattribute__` is called for every attribute access, regardless of whether the attribute exists or not. It is invoked before the usual attribute lookup mechanism and can be used to intercept and modify attribute access.

Q2. Properties and descriptors are both mechanisms in Python that allow customization of attribute access, but they differ in their implementation and behavior:
- Properties: Properties are a high-level way to define computed or calculated attributes. They use special methods (`getter`, `setter`, `deleter`) to define the behavior of attribute access and modification. Properties are bound to a specific class attribute and are accessed like regular attributes, but the attribute access triggers the corresponding property methods.
- Descriptors: Descriptors are a low-level mechanism for defining attribute access and modification behavior. They are objects that define special methods (`__get__`, `__set__`, `__delete__`) and can be assigned to class attributes. When an attribute with a descriptor is accessed or modified, the descriptor's methods are called to handle the operation. Descriptors provide more fine-grained control over attribute access and can be reused across different attributes and classes.

Q3. The key differences in functionality between `__getattr__` and `__getattribute__`, as well as properties and descriptors, can be summarized as follows:
- `__getattr__`: It is called only when an attribute is not found through normal lookup. It allows defining a fallback behavior for attribute access failures. It is typically used to handle non-existent or dynamically generated attributes.
- `__getattribute__`: It is called for every attribute access, regardless of whether the attribute exists or not. It allows intercepting and modifying attribute access before the usual lookup mechanism takes place. It is typically used for attribute access control or customization.
- Properties: They provide a high-level way to define computed or calculated attributes. They allow defining custom behavior for attribute access, modification, and deletion using the `getter`, `setter`, and `deleter` methods. Properties are accessed and assigned like regular attributes.
- Descriptors: They provide a low-level mechanism for defining attribute access and modification behavior. They are objects assigned to class attributes and define the `__get__`, `__set__`, and `__delete__` methods. Descriptors allow fine-grained control over attribute access and can be reused across different attributes and classes. They are accessed and assigned through the descriptor protocol.

Overall, `__getattr__` and `__getattribute__` are used for attribute access customization, while properties and descriptors provide different levels of abstraction and flexibility in defining attribute behavior.