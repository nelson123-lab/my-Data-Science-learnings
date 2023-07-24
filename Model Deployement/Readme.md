To deploy our model in production map. So we need to export our model and bind with web application API.

Pickle is the standard way of serializing objects in Python. You can use the pickle operation to serialize your machine 
learning algorithms and save the serialized format to a file. Later you can load this file to deserialize your model and use it 
to make new predictions

```python
model.fit(X_train, Y_train)
# save the model to disk
filename = 'finalized_model.sav'
pickle.dump(model, open(filename, 'wb'))

# some time later...

# load the model from disk
loaded_model = pickle.load(open(filename, 'rb'))
result = loaded_model.score(X_test, Y_test)
print(result)

```
