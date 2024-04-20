# Problem: User Role as "ANONYMOUS"

## Solution:
The default user role "anonymous" isn't valid for database entries. To resolve this, I adjusted the default user role to "user" within the user_model.py file.

>>> role: Mapped[UserRole] = Column(SQLAlchemyEnum(UserRole), default=UserRole.USER, nullable=False)
