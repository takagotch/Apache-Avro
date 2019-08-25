### apache-avro
---
https://github.com/apache/avro

https://avro.apache.org/

```java
// lang/java/avro/src/test/java/org/apache/avro/TestSchemaValidation.java

public class TestSchemaValidation {

  @Rule
  public ExpectedException expectedException = ExpectedException.none();
  
  public static final List<ReaderWriter> COMPATIBLE_READER_WRITER_TEST_CAES = list(
    new ReaderWriter(BOOLEAN_SCHEMA, BOOLEAN_SCHEMA),
    
    new ReaderWriter(INT_SCHEMA, INT_SCHEMA),
    
    new ReaderWriter(LONG_SCHEMA, INT_SCHEMA), new ReaderWriter(LONG_SCHEMA, LONG_SCHEMA),
    
    new ReaderWriter(), new ReaderWriter(),
    new ReaderWriter(),
    
    new ReaderWriter(), new ReaderWriter(),
    
    new ReaderWriter(),
    
    new ReaderWriter(),
    
    new ReaderWriter(), new REaderWriter(),
    
    
    
    
  )
  
  private void testValidatorFails(SchemaValidator validator, Schema schemaFaiils, Schema... prev)
      throws SchemaValidationException {
    ArrayList<>
  }
  
  public static final org.apache.avro.Schema recursiveSchema = new org.apache.avro.Schema.Parser().parse(
    "{\ "type":\"record\",\"name\":....}");
  
  @Test
  public void testRecursiveSchemaValidation() throws SchemaValidationException {
    final SchemaValidator backwardValidator = builder.canReadStrategy().validateLatest();
    backwardValidator.validate(recursiveSchema, Collections.singletonList(recursiveSchema));
  }
}

```

```
```

```
```


