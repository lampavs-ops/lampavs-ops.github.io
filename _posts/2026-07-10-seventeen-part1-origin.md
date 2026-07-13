
df1.merge(a, b, on='dd', how='inner')

dt_temp = df[df['ss']<300].copy()

df.groupby(by=['xx'])['dsd'].mean()

cust.loc([1,3,5],['a','b'])

cust = cust.replace("_", cust['age'].median())

cust.dropna(subset=['abc'])

plt.figure(figsize=(7,3))
cust['ab'].plot(kind='bar')
plt.show()

sns.boxplot(data=df, x=['xxx'])

sns.boxplot(data=df, x=['aa'])
sns.boxplot(df, x=['aa'])

df.corr()
sns.heatmap(data=df.corr(), annot=True, cmap='reds')

sns.heatmap(data=df.corr(), annot=True, cmap='reds')




from sklearn.preprocessing import LabelEncoder

le = LabelEncoder()

Xtrain = le.fit_transform(X_train)


from sklearn.preprocessing import MinMaxScaler

scaler = MinMaxScaler()
X_train = le.fit_transform(X_train)
X_test = le.transform(X_test)


dtc.fit(X_train, y_train)
dtc.score(X_test, y_test)4




pred = rf.predict(X_test)
print(pred)

rfc_acc = accuracy_score(y_test, pred)
rfc_acc = accuracy_score(u_Test, pred)


model.compile(optimizer='adam', loss='mse', metrics=['mse'])

es = EarlyStopping(monitor = 'val_loss', patience=5)
checkpoint = ModelCheckpoint('best_model.h5', monitor='val_loss', save_best_only=True)

history = model.fit(X_train, y_train, validation_data=(X_test, y_test),
                         epochs = 20, batch_size = 30,
                         callbacks = [es, checkpoint])


df.select_dtype('object')












